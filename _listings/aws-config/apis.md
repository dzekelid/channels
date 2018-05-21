---
name: AWS Config
x-slug: aws-config
description: AWS Config is a fully managed service that provides you with an AWS resource
  inventory, configuration history, and configuration change notifications to enable
  security and governance. Config Rules enables you to create rules that automatically
  check the configuration of AWS resources recorded by AWS Config.With AWS Config,
  you can discover existing and deleted AWS resources, determine your overall compliance
  against rules, and dive into configuration details of a resource at any point in
  time. These capabilities enable compliance auditing, security analysis, resource
  change tracking, and troubleshooting.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
x-kinRank: "10"
x-alexaRank: ""
tags: Channels
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/aws-config/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Config API Delete Delivery Channel
  x-api-slug: aws-config-api
  description: Deletes the delivery channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: ://///?Action=DeleteDeliveryChannel
  tags: Delivery Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/aws-config/actiondeletedeliverychannel-get-openapi.md
- name: AWS Config API Describe Delivery Channels
  x-api-slug: aws-config-api
  description: Returns details about the specified delivery channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: ://///?Action=DescribeDeliveryChannels
  tags: Delivery Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/aws-config/actiondescribedeliverychannels-get-openapi.md
- name: AWS Config API Describe Delivery Channel Status
  x-api-slug: aws-config-api
  description: Returns the current status of the specified delivery channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: ://///?Action=DescribeDeliveryChannelStatus
  tags: Delivery Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/aws-config/actiondescribedeliverychannelstatus-get-openapi.md
- name: AWS Config API Put Delivery Channel
  x-api-slug: aws-config-api
  description: Creates a delivery channel object to deliver configuration information
    to an Amazon S3 bucket and Amazon SNS topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: ://///?Action=PutDeliveryChannel
  tags: Delivery Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/aws-config/actionputdeliverychannel-get-openapi.md
- name: AWS Config API
  x-api-slug: aws-config-api
  description: AWS Config is a fully managed service that provides you with an AWS
    resource inventory, configuration history, and configuration change notifications
    to enable security and governance. Config Rules enables you to create rules that
    automatically check the configuration of AWS resources recorded by AWS Config.With
    AWS Config, you can discover existing and deleted AWS resources, determine your
    overall compliance against rules, and dive into configuration details of a resource
    at any point in time. These capabilities enable compliance auditing, security
    analysis, resource change tracking, and troubleshooting.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/channels/master/_listings/aws-config/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/configservice/index.html
- type: x-console
  url: https://console.aws.amazon.com/config
- type: x-documentation
  url: http://docs.aws.amazon.com/config/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/config/faq/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=184
- type: x-getting-started
  url: https://aws.amazon.com/config/getting-started/
- type: x-partners
  url: https://aws.amazon.com/config/partners/
- type: x-pricing
  url: https://aws.amazon.com/config/pricing/
- type: x-support
  url: https://console.aws.amazon.com/support/
- type: x-website
  url: https://aws.amazon.com/config/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---