---
name: AWS Elastic Beanstalk
x-slug: aws-elastic-beanstalk
description: AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling
  web applications and services developed with Java,.NET, PHP, Node.js, Python, Ruby,
  Go, andDockeron familiar servers such as Apache, Nginx, Passenger, andIIS.You can
  simply upload your code and Elastic Beanstalk automatically handles the deployment,
  from capacity provisioning, load balancing, auto-scaling to application health monitoring.
  At the same time, you retain full control over the AWS resources powering your application
  and can access the underlying resources at any time.There is no additional charge
  for Elastic Beanstalk - you pay only for the AWS resources needed to store and run
  your applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AWSElasticBeanstalk.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Templates
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/aws-elastic-beanstalk/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Elastic Beanstalk API Create Configuration Template
  x-api-slug: aws-elastic-beanstalk-api
  description: Creates a configuration template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AWSElasticBeanstalk.png
  humanURL: https://aws.amazon.com/elasticbeanstalk/
  baseURL: ://///?Action=CreateConfigurationTemplate
  tags: Configuration Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/aws-elastic-beanstalk/actioncreateconfigurationtemplate-get-openapi.md
- name: AWS Elastic Beanstalk API Delete Configuration Template
  x-api-slug: aws-elastic-beanstalk-api
  description: Deletes the specified configuration template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AWSElasticBeanstalk.png
  humanURL: https://aws.amazon.com/elasticbeanstalk/
  baseURL: ://///?Action=DeleteConfigurationTemplate
  tags: Configuration Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/aws-elastic-beanstalk/actiondeleteconfigurationtemplate-get-openapi.md
- name: AWS Elastic Beanstalk API Update Configuration Template
  x-api-slug: aws-elastic-beanstalk-api
  description: |-
    Updates the specified configuration template to have the specified properties or
          configuration option values.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AWSElasticBeanstalk.png
  humanURL: https://aws.amazon.com/elasticbeanstalk/
  baseURL: ://///?Action=UpdateConfigurationTemplate
  tags: Configuration Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/aws-elastic-beanstalk/actionupdateconfigurationtemplate-get-openapi.md
- name: AWS Elastic Beanstalk API
  x-api-slug: aws-elastic-beanstalk-api
  description: AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling
    web applications and services developed with Java,.NET, PHP, Node.js, Python,
    Ruby, Go, andDockeron familiar servers such as Apache, Nginx, Passenger, andIIS.You
    can simply upload your code and Elastic Beanstalk automatically handles the deployment,
    from capacity provisioning, load balancing, auto-scaling to application health
    monitoring. At the same time, you retain full control over the AWS resources powering
    your application and can access the underlying resources at any time.There is
    no additional charge for Elastic Beanstalk - you pay only for the AWS resources
    needed to store and run your applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AWSElasticBeanstalk.png
  humanURL: https://aws.amazon.com/elasticbeanstalk/
  baseURL: :///
  tags: Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/templates/master/_listings/aws-elastic-beanstalk/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/AWS-Elastic-Beanstalk
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3.html
- type: x-documentation
  url: http://docs.aws.amazon.com/elasticbeanstalk/latest/api/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/elasticbeanstalk/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=86
- type: x-getting-started
  url: https://aws.amazon.com/elasticbeanstalk/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticbeanstalk/pricing/
- type: x-website
  url: https://aws.amazon.com/elasticbeanstalk/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---