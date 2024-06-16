# Frontend for AWS Developer course (RS School)

## [Task 3] Add backend using AWS Lambdas and API Gateway - CURRENT STEP

### Links

* Task: https://github.com/rolling-scopes-school/aws/blob/main/aws-developer/03_serverless_api/task.md
* cloudfront: https://d2bk3wwmc4t4q2.cloudfront.net/
* GitHub repos (`task-3` branch):
  * back-end: https://github.com/deniskarandashev/aws-shop-be
  * front-end: https://github.com/deniskarandashev/nodejs-aws-shop-react
* Requests: 
  * GET /products: https://sfn070sct9.execute-api.eu-north-1.amazonaws.com/prod/products
  * GET /products/{productId}: https://sfn070sct9.execute-api.eu-north-1.amazonaws.com/prod/products/10
* Pull requests:
  * back-end: https://github.com/deniskarandashev/aws-shop-be/pull/1
  * front-end: https://github.com/deniskarandashev/nodejs-aws-shop-react/pull/2
* Swagger:
  * local:
    * swagger ui: http://localhost:8080/swagger-ui/index.html 
    * api-docs: http://localhost:8080/v3/api-docs
  * `openapi.json` in the root of back-end project (`task-3` branch) contains code that can be rendered by https://editor.swagger.io/

### Estimation (self-estimation: 100/100)

* #### Main [70/70]
[+] Product Service contains configuration for 2 lambda functions, API is not working at all, but configuration is correct

[+] The getProductsList OR getProductsById lambda function returns a correct response (POINT1)

[+] The getProductsById AND getProductsList lambda functions return a correct response code (POINT2)

[+] Your own Frontend application is integrated with Product Service (/products API) and products from Product Service are represented on Frontend. AND POINT1 and POINT2 are done.

* #### Additional [30/30]
[+] +7.5 (All languages) - Swagger documentation is created for Product Service. This can be, for example, openapi.(json|yaml) added to the repository, that can be rendered by https://editor.swagger.io/

[+] +7.5 (All languages) - Lambda handlers are covered by basic UNIT tests (NO infrastructure logic is needed to be covered)

[+] +7.5 (All languages) - Lambda handlers (getProductsList, getProductsById) code is written not in 1 single module (file) and separated in codebase.

[+] +7.5 (All languages) - Main error scenarios are handled by API ("Product not found" error).

## [Task 2] React-shop-cloudfront - ARCHIVED STEP

_NOTE: info below might be outdated because of next steps._

### Links 

* cloudfront: https://dike63j25qf7o.cloudfront.net
* s3: http://awsstack-deploymentfrontendawsbucketc2ffaf4a-qy7lnix22sny.s3-website.eu-north-1.amazonaws.com


### Estimation (self-estimation: 100/100)

[+] - **30** - S3 bucket has been created and configured properly. The app has been uploaded to the bucket and is available though the Internet. Nothing else has been done.
  _(Link to S3 bucket/website is provided. There is no Pull Request in the YOUR OWN frontend repository.)_

[+] - **40** - In addition to the previous work a CloudFront distribution is created and configured properly and the site is served now with CloudFront and is available through the Internet over CloudFront URL, not S3-website link (due to changes in bucket’s policy...).
  _(Link to CloudFront website is provided. S3-website shows 403 Access Denied error. There is no Pull Request in the YOUR OWN frontend repository.)_

[+] - **30** - S3 bucket creation, website deployment, CloudFront Distribution and Invalidation added and configured by using AWS CDK. The app can be built and deployed by running npm script command.
  _(Link to CloudFront website is provided. PR with all changes is submitted in the YOUR OWN frontend repository and its link is provided for review.)_