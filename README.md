# Cloudformation s3 cloudfront template
This template creates s3 bucket for angular app > 4.x like static web hosting and cloudfront distribution which based on s3 bucket.

## Params
| Name | Type | Description |
|:------ |:-----|:-----------------|
| **AcmCertificateArn**| `string`<br/>*required* | Amazon Resource Name (ARN) of an AWS Certificate Manager (ACM) certificate. Certificate must be uploaded to N.Virginia
| **appName**| `string`<br/>*required* | The name of subdomain e.g app or app-dev or app-stating
| **domainName**| `string`<br/>*required* | Domain name e.g test.com

In the end of process will be created s3 bucket and cloudfront distrubution with alias like {appName}.{domainName} e.g app-dev.test.com.

Template setup s3 static web hosting for angular app > 4.x