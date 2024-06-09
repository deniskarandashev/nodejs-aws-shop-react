## React-shop-cloudfront

### Links 

cloudfront: https://dike63j25qf7o.cloudfront.net

s3: http://awsstack-deploymentfrontendawsbucketc2ffaf4a-qy7lnix22sny.s3-website.eu-north-1.amazonaws.com


### Estimation (self-estimation: 100/100)

[+] - **30** - S3 bucket has been created and configured properly. The app has been uploaded to the bucket and is available though the Internet. Nothing else has been done.
  _(Link to S3 bucket/website is provided. There is no Pull Request in the YOUR OWN frontend repository.)_

[+] - **40** - In addition to the previous work a CloudFront distribution is created and configured properly and the site is served now with CloudFront and is available through the Internet over CloudFront URL, not S3-website link (due to changes in bucket’s policy...).
  _(Link to CloudFront website is provided. S3-website shows 403 Access Denied error. There is no Pull Request in the YOUR OWN frontend repository.)_

[+] - **30** - S3 bucket creation, website deployment, CloudFront Distribution and Invalidation added and configured by using AWS CDK. The app can be built and deployed by running npm script command.
  _(Link to CloudFront website is provided. PR with all changes is submitted in the YOUR OWN frontend repository and its link is provided for review.)_