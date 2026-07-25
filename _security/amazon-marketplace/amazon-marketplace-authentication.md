---
api_key_in:
- header
api_specs:
- filename: amazon-marketplace-cancelchangeset-catalog-changesetid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace CancelChangeSet#catalog&changeSetId API
  slug: amazon-marketplace-cancelchangeset-catalog-changesetid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-cancelchangeset-catalog-changesetid-api-openapi.yml
- filename: amazon-marketplace-deleteresourcepolicy-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DeleteResourcePolicy#resourceArn API
  slug: amazon-marketplace-deleteresourcepolicy-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-deleteresourcepolicy-resourcearn-api-openapi.yml
- filename: amazon-marketplace-describechangeset-catalog-changesetid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DescribeChangeSet#catalog&changeSetId API
  slug: amazon-marketplace-describechangeset-catalog-changesetid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-describechangeset-catalog-changesetid-api-openapi.yml
- filename: amazon-marketplace-describeentity-catalog-entityid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DescribeEntity#catalog&entityId API
  slug: amazon-marketplace-describeentity-catalog-entityid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-describeentity-catalog-entityid-api-openapi.yml
- filename: amazon-marketplace-getresourcepolicy-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon Marketplace GetResourcePolicy#resourceArn API
  slug: amazon-marketplace-getresourcepolicy-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-getresourcepolicy-resourcearn-api-openapi.yml
- filename: amazon-marketplace-listchangesets-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListChangeSets API
  slug: amazon-marketplace-listchangesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listchangesets-api-openapi.yml
- filename: amazon-marketplace-listentities-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListEntities API
  slug: amazon-marketplace-listentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listentities-api-openapi.yml
- filename: amazon-marketplace-listtagsforresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListTagsForResource API
  slug: amazon-marketplace-listtagsforresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listtagsforresource-api-openapi.yml
- filename: amazon-marketplace-putresourcepolicy-api-openapi.yml
  format: yaml
  label: Amazon Marketplace PutResourcePolicy API
  slug: amazon-marketplace-putresourcepolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-putresourcepolicy-api-openapi.yml
- filename: amazon-marketplace-startchangeset-api-openapi.yml
  format: yaml
  label: Amazon Marketplace StartChangeSet API
  slug: amazon-marketplace-startchangeset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-startchangeset-api-openapi.yml
- filename: amazon-marketplace-tagresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace TagResource API
  slug: amazon-marketplace-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-tagresource-api-openapi.yml
- filename: amazon-marketplace-untagresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace UntagResource API
  slug: amazon-marketplace-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-untagresource-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Marketplace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Marketplace secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-marketplace-openapi-original.yaml
  type: apiKey
slug: amazon-marketplace-authentication
source_filename: amazon-marketplace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-marketplace-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-marketplace-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/authentication/amazon-marketplace-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
---
