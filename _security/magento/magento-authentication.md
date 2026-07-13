---
api_key_in: []
api_specs:
- filename: magento-rest-api-openapi.yml
  format: yaml
  label: Magento REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-rest-api-openapi.yml
- filename: magento-webhooks-asyncapi.yml
  format: yaml
  label: Adobe Commerce Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/asyncapi/magento-webhooks-asyncapi.yml
- filename: magento-events-asyncapi.yml
  format: yaml
  label: Adobe Commerce Eventing
  slug: events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/asyncapi/magento-events-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Magento Authentication
name_suffix: Authentication
oauth_flows: []
overview: magento secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: magento
provider_slug: magento
scheme_count: 1
schemes:
- description: Bearer token obtained from the /V1/integration/admin/token or /V1/integration/customer/token endpoint. Include in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/magento-rest-api-openapi.yml
  type: http
slug: magento-authentication
source_filename: magento-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magento-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the /V1/integration/admin/token or /V1/integration/customer/token\n    endpoint. Include in the Authorization header as \"Bearer {token}\".\n  sources:\n  - openapi/magento-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/authentication/magento-authentication.yml
summary_line: http · 1 scheme
tags: []
---
