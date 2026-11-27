---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: terminal49-shipping-lines-api-openapi.yml
  format: yaml
  label: Terminal49 Shipping Lines API
  slug: terminal49-shipping-lines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-shipping-lines-api-openapi.yml
- filename: terminal49-terminals-api-openapi.yml
  format: yaml
  label: Terminal49 Terminals API
  slug: terminal49-terminals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-terminals-api-openapi.yml
- filename: terminal49-tracking-requests-api-openapi.yml
  format: yaml
  label: Terminal49 Tracking Requests API
  slug: terminal49-tracking-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-tracking-requests-api-openapi.yml
- filename: terminal49-transport-events-api-openapi.yml
  format: yaml
  label: Terminal49 Transport Events API
  slug: terminal49-transport-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-transport-events-api-openapi.yml
- filename: terminal49-webhooks-api-openapi.yml
  format: yaml
  label: Terminal49 Webhooks API
  slug: terminal49-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-webhooks-api-openapi.yml
- filename: terminal49-containers-api-openapi.yml
  format: yaml
  label: Terminal49 Containers API
  slug: terminal49-containers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-containers-api-openapi.yml
- filename: terminal49-custom-field-definitions-api-openapi.yml
  format: yaml
  label: Terminal49 Custom Field Definitions API
  slug: terminal49-custom-field-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-custom-field-definitions-api-openapi.yml
- filename: terminal49-custom-field-options-api-openapi.yml
  format: yaml
  label: Terminal49 Custom Field Options API
  slug: terminal49-custom-field-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-custom-field-options-api-openapi.yml
- filename: terminal49-custom-fields-api-openapi.yml
  format: yaml
  label: Terminal49 Custom Fields API
  slug: terminal49-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-custom-fields-api-openapi.yml
- filename: terminal49-document-schemas-api-openapi.yml
  format: yaml
  label: Terminal49 Document Schemas API
  slug: terminal49-document-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-document-schemas-api-openapi.yml
- filename: terminal49-documents-api-openapi.yml
  format: yaml
  label: Terminal49 Documents API
  slug: terminal49-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-documents-api-openapi.yml
- filename: terminal49-email-submissions-api-openapi.yml
  format: yaml
  label: Terminal49 Email Submissions API
  slug: terminal49-email-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-email-submissions-api-openapi.yml
- filename: terminal49-metro-areas-api-openapi.yml
  format: yaml
  label: Terminal49 Metro Areas API
  slug: terminal49-metro-areas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-metro-areas-api-openapi.yml
- filename: terminal49-parties-api-openapi.yml
  format: yaml
  label: Terminal49 Parties API
  slug: terminal49-parties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-parties-api-openapi.yml
- filename: terminal49-ports-api-openapi.yml
  format: yaml
  label: Terminal49 Ports API
  slug: terminal49-ports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-ports-api-openapi.yml
- filename: terminal49-routing-paid-api-openapi.yml
  format: yaml
  label: Terminal49 Routing (Paid) API
  slug: terminal49-routing-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-routing-paid-api-openapi.yml
- filename: terminal49-search-api-openapi.yml
  format: yaml
  label: Terminal49 Search API
  slug: terminal49-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-search-api-openapi.yml
- filename: terminal49-shipments-api-openapi.yml
  format: yaml
  label: Terminal49 Shipments API
  slug: terminal49-shipments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-shipments-api-openapi.yml
- filename: terminal49-vessels-api-openapi.yml
  format: yaml
  label: Terminal49 Vessels API
  slug: terminal49-vessels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-vessels-api-openapi.yml
- filename: terminal49-webhook-notifications-api-openapi.yml
  format: yaml
  label: Terminal49 Webhook Notifications API
  slug: terminal49-webhook-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal49/openapi/terminal49-webhook-notifications-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Terminal49 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminal49 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terminal49
provider_slug: terminal49
scheme_count: 1
schemes:
- description: 'Token-based authentication. Send the header `Authorization: Token YOUR_API_KEY`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/terminal49-openapi.yml
  type: apiKey
slug: terminal49-authentication
source_filename: terminal49-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/terminal49-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Send the header `Authorization: Token YOUR_API_KEY`.'\n  sources:\n  - openapi/terminal49-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/terminal49/authentication/terminal49-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Container Tracking
- Ocean Freight
- Supply Chain
- Logistics
- Shipping
- Freight
---
