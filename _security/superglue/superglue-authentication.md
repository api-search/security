---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: superglue-connections-api-openapi.yml
  format: yaml
  label: Index Commerce Connections API
  slug: superglue-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-connections-api-openapi.yml
- filename: superglue-runs-api-openapi.yml
  format: yaml
  label: Index Commerce Runs API
  slug: superglue-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-runs-api-openapi.yml
- filename: superglue-tools-api-openapi.yml
  format: yaml
  label: Index Commerce Tools API
  slug: superglue-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-tools-api-openapi.yml
- filename: superglue-webhooks-api-openapi.yml
  format: yaml
  label: Index Commerce Webhooks API
  slug: superglue-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superglue/openapi/superglue-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Superglue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Index Commerce secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Index Commerce
provider_slug: superglue
scheme_count: 2
schemes:
- bearerFormat: Static API Key
  description: 'Send a superglue API key in the Authorization header:

    `Authorization: Bearer YOUR_API_KEY`.


    Create and manage API keys from **API Keys** in the organization menu.'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/superglue-openapi.yml
  type: http
- description: 'Query-string authentication for webhook providers that cannot set an Authorization header.

    The complete webhook URL contains a secret and must be protected accordingly.'
  in: query
  name: WebhookTokenAuth
  parameter: token
  sources:
  - openapi/superglue-openapi.yml
  type: apiKey
slug: superglue-authentication
source_filename: superglue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/superglue-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Static API Key\n  description: |-\n    Send a superglue API key in the Authorization header:\n    `Authorization: Bearer YOUR_API_KEY`.\n\n    Create and manage API keys from **API Keys** in the organization menu.\n  sources:\n  - openapi/superglue-openapi.yml\n- name: WebhookTokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: |-\n    Query-string authentication for webhook providers that cannot set an Authorization header.\n    The complete webhook URL contains a secret and must be protected accordingly.\n  sources:\n  - openapi/superglue-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/superglue/authentication/superglue-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- E-Commerce
- Platform
- Storefront
- Analytics
---
