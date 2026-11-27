---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getbioflow-com-analytics-api-openapi.yml
  format: yaml
  label: BioFlow Analytics API
  slug: getbioflow-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getbioflow-com/openapi/getbioflow-com-analytics-api-openapi.yml
- filename: getbioflow-com-contacts-api-openapi.yml
  format: yaml
  label: BioFlow Contacts API
  slug: getbioflow-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getbioflow-com/openapi/getbioflow-com-contacts-api-openapi.yml
- filename: getbioflow-com-files-api-openapi.yml
  format: yaml
  label: BioFlow Files API
  slug: getbioflow-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getbioflow-com/openapi/getbioflow-com-files-api-openapi.yml
- filename: getbioflow-com-pages-api-openapi.yml
  format: yaml
  label: BioFlow Pages API
  slug: getbioflow-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getbioflow-com/openapi/getbioflow-com-pages-api-openapi.yml
- filename: getbioflow-com-usage-api-openapi.yml
  format: yaml
  label: BioFlow Usage API
  slug: getbioflow-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getbioflow-com/openapi/getbioflow-com-usage-api-openapi.yml
- filename: getbioflow-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: BioFlow Webhook Endpoints API
  slug: getbioflow-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getbioflow-com/openapi/getbioflow-com-webhook-endpoints-api-openapi.yml
auth_types: []
description: Authentication schemes as published on BioFlow docs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: BioFlow Authentication
name_suffix: Authentication
oauth_flows: []
overview: BioFlow declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BioFlow
provider_slug: getbioflow-com
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer bf_live_YOUR_KEY'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'x-api-key: bf_live_YOUR_KEY'
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
slug: getbioflow-com-authentication
source_filename: getbioflow-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getbioflow.com/docs/api-reference/rotateWebhookSecret
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getbioflow.com/docs/api-reference/rotateWebhookSecret\nsources:\n- https://getbioflow.com/docs/api-reference/rotateWebhookSecret\n- https://getbioflow.com/docs/api\n- https://getbioflow.com/agent-setup.md\ndescription: Authentication schemes as published on BioFlow docs\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer bf_live_YOUR_KEY'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: x-api-key\n  evidence: 'x-api-key: bf_live_YOUR_KEY'\n  location: header\n  header: x-api-key\nnote: No OAuth2, JWT, HMAC, MTLS, or other schemes are documented on the provided pages.\ndocs: https://getbioflow.com/docs/api-reference/rotateWebhookSecret\n"
source_yaml_url: https://artifacts.apis.io/getbioflow-com/authentication/getbioflow-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Link-in-bio
- Page Builder
- No-Code
- Free Tier
---
