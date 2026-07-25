---
api_key_in:
- header
api_specs:
- filename: amazon-mq-broker-engine-types-api-openapi.yml
  format: yaml
  label: Amazon MQ Broker Engine Types API
  slug: amazon-mq-broker-engine-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/openapi/amazon-mq-broker-engine-types-api-openapi.yml
- filename: amazon-mq-broker-instance-options-api-openapi.yml
  format: yaml
  label: Amazon MQ Broker Instance Options API
  slug: amazon-mq-broker-instance-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/openapi/amazon-mq-broker-instance-options-api-openapi.yml
- filename: amazon-mq-brokers-api-openapi.yml
  format: yaml
  label: Amazon MQ Brokers API
  slug: amazon-mq-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/openapi/amazon-mq-brokers-api-openapi.yml
- filename: amazon-mq-configurations-api-openapi.yml
  format: yaml
  label: Amazon MQ Configurations API
  slug: amazon-mq-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/openapi/amazon-mq-configurations-api-openapi.yml
- filename: amazon-mq-tags-api-openapi.yml
  format: yaml
  label: Amazon MQ Tags API
  slug: amazon-mq-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/openapi/amazon-mq-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MQ
provider_slug: amazon-mq
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mq-openapi-original.yml
  type: apiKey
slug: amazon-mq-authentication
source_filename: amazon-mq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mq-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mq-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/authentication/amazon-mq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
