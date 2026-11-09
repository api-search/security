---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-ads-openapi-generated.yml
  format: yaml
  label: Amazon Ads API
  slug: amazon-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/_ae-authored/amazon-ads-openapi-generated.yml
- filename: amazon-ads-activategiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Activategiftcard API
  slug: amazon-ads-activategiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-activategiftcard-api-openapi.yml
- filename: amazon-ads-activationstatuscheck-api-openapi.yml
  format: yaml
  label: Amazon Ads Activationstatuscheck API
  slug: amazon-ads-activationstatuscheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-activationstatuscheck-api-openapi.yml
- filename: amazon-ads-amazon-ads-api-api-openapi.yml
  format: yaml
  label: Amazon Ads Amazon Ads API
  slug: amazon-ads-amazon-ads-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-amazon-ads-api-api-openapi.yml
- filename: amazon-ads-cancelgiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Cancelgiftcard API
  slug: amazon-ads-cancelgiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-cancelgiftcard-api-openapi.yml
- filename: amazon-ads-creategiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Creategiftcard API
  slug: amazon-ads-creategiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-creategiftcard-api-openapi.yml
- filename: amazon-ads-deactivategiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Deactivategiftcard API
  slug: amazon-ads-deactivategiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-deactivategiftcard-api-openapi.yml
- filename: amazon-ads-getgiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Getgiftcard API
  slug: amazon-ads-getgiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-getgiftcard-api-openapi.yml
- filename: amazon-ads-install-api-openapi.yml
  format: yaml
  label: Amazon Ads Install API
  slug: amazon-ads-install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-install-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Ads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Ads secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Ads
provider_slug: amazon-ads
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/amazon-ads-activategiftcard-api-openapi.yml
  - openapi/amazon-ads-activationstatuscheck-api-openapi.yml
  - openapi/amazon-ads-amazon-ads-api-api-openapi.yml
  - openapi/amazon-ads-cancelgiftcard-api-openapi.yml
  - openapi/amazon-ads-creategiftcard-api-openapi.yml
  - openapi/amazon-ads-deactivategiftcard-api-openapi.yml
  - openapi/amazon-ads-getgiftcard-api-openapi.yml
  - openapi/amazon-ads-install-api-openapi.yml
  type: apiKey
slug: amazon-ads-authentication
source_filename: amazon-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/amazon-ads-activategiftcard-api-openapi.yml, openapi/amazon-ads-activationstatuscheck-api-openapi.yml,\n  openapi/amazon-ads-amazon-ads-api-api-openapi.yml, openapi/amazon-ads-cancelgiftcard-api-openapi.yml,\n  openapi/amazon-ads-creategiftcard-api-openapi.yml, openapi/amazon-ads-deactivategiftcard-api-openapi.yml,\n  openapi/amazon-ads-getgiftcard-api-openapi.yml, openapi/amazon-ads-install-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/amazon-ads-activategiftcard-api-openapi.yml\n  - openapi/amazon-ads-activationstatuscheck-api-openapi.yml\n  - openapi/amazon-ads-amazon-ads-api-api-openapi.yml\n  - openapi/amazon-ads-cancelgiftcard-api-openapi.yml\n  - openapi/amazon-ads-creategiftcard-api-openapi.yml\n  - openapi/amazon-ads-deactivategiftcard-api-openapi.yml\n  - openapi/amazon-ads-getgiftcard-api-openapi.yml\n\
  \  - openapi/amazon-ads-install-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-ads/authentication/amazon-ads-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Advertising
- Marketing
- Amazon
- Technology
- Software-as-a-Service
---
