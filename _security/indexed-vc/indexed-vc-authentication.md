---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: indexed-vc-companies-api-openapi.yml
  format: yaml
  label: Indexed Companies API
  slug: indexed-vc-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-companies-api-openapi.yml
- filename: indexed-vc-enrich-api-openapi.yml
  format: yaml
  label: Indexed Enrich API
  slug: indexed-vc-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-enrich-api-openapi.yml
- filename: indexed-vc-industries-api-openapi.yml
  format: yaml
  label: Indexed Industries API
  slug: indexed-vc-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-industries-api-openapi.yml
- filename: indexed-vc-investors-api-openapi.yml
  format: yaml
  label: Indexed Investors API
  slug: indexed-vc-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-investors-api-openapi.yml
- filename: indexed-vc-reveal-api-openapi.yml
  format: yaml
  label: Indexed Reveal API
  slug: indexed-vc-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-reveal-api-openapi.yml
- filename: indexed-vc-scheduled-exports-api-openapi.yml
  format: yaml
  label: Indexed Scheduled Exports API
  slug: indexed-vc-scheduled-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-scheduled-exports-api-openapi.yml
- filename: indexed-vc-usage-api-openapi.yml
  format: yaml
  label: Indexed Usage API
  slug: indexed-vc-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-usage-api-openapi.yml
- filename: indexed-vc-webhooks-api-openapi.yml
  format: yaml
  label: Indexed Webhooks API
  slug: indexed-vc-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/openapi/indexed-vc-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Indexed Vc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indexed secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Indexed
provider_slug: indexed-vc
scheme_count: 1
schemes:
- description: API key in format `idx_<32chars>`. Available on every plan; entity detail and reveal spend credits on every plan, while bulk enrichment, webhooks, scheduled exports and listing/sorting require a paid plan (Silver+).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/indexed-vc-openapi.yaml
  type: apiKey
slug: indexed-vc-authentication
source_filename: indexed-vc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: derived\nsource: openapi/indexed-vc-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key in format `idx_<32chars>`. Available on every plan; entity detail and\n    reveal spend credits on every plan, while bulk enrichment, webhooks, scheduled exports and\n    listing/sorting require a paid plan (Silver+).\n  sources:\n  - openapi/indexed-vc-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indexed-vc/refs/heads/main/authentication/indexed-vc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Private Company
- Funding
---
