---
api_key_in:
- header
api_specs:
- filename: amazon-msk-clusters-api-openapi.yml
  format: yaml
  label: Amazon MSK Clusters API
  slug: amazon-msk-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-clusters-api-openapi.yml
- filename: amazon-msk-compatible-kafka-versions-api-openapi.yml
  format: yaml
  label: Amazon MSK Compatible Kafka Versions API
  slug: amazon-msk-compatible-kafka-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-compatible-kafka-versions-api-openapi.yml
- filename: amazon-msk-configurations-api-openapi.yml
  format: yaml
  label: Amazon MSK Configurations API
  slug: amazon-msk-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-configurations-api-openapi.yml
- filename: amazon-msk-kafka-versions-api-openapi.yml
  format: yaml
  label: Amazon MSK Kafka Versions API
  slug: amazon-msk-kafka-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-kafka-versions-api-openapi.yml
- filename: amazon-msk-operations-api-openapi.yml
  format: yaml
  label: Amazon MSK Operations API
  slug: amazon-msk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-operations-api-openapi.yml
- filename: amazon-msk-tags-api-openapi.yml
  format: yaml
  label: Amazon MSK Tags API
  slug: amazon-msk-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/openapi/amazon-msk-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Msk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MSK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MSK
provider_slug: amazon-msk
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-msk-openapi-original.yml
  type: apiKey
slug: amazon-msk-authentication
source_filename: amazon-msk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-msk-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-msk-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/authentication/amazon-msk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
