---
anonymous_access: false
api_key_in: []
api_specs:
- filename: companydata-dk-account-api-openapi.yml
  format: yaml
  label: companydata.dk Account API
  slug: companydata-dk-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-account-api-openapi.yml
- filename: companydata-dk-auditors-api-openapi.yml
  format: yaml
  label: companydata.dk Auditors API
  slug: companydata-dk-auditors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-auditors-api-openapi.yml
- filename: companydata-dk-companies-api-openapi.yml
  format: yaml
  label: companydata.dk Companies API
  slug: companydata-dk-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-companies-api-openapi.yml
- filename: companydata-dk-cvrapi-dk-compatibility-api-openapi.yml
  format: yaml
  label: companydata.dk cvrapi.dk compatibility API
  slug: companydata-dk-cvrapi-dk-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-cvrapi-dk-compatibility-api-openapi.yml
- filename: companydata-dk-e-invoicing-api-openapi.yml
  format: yaml
  label: companydata.dk E Invoicing API
  slug: companydata-dk-e-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-e-invoicing-api-openapi.yml
- filename: companydata-dk-legal-notices-api-openapi.yml
  format: yaml
  label: companydata.dk Legal notices API
  slug: companydata-dk-legal-notices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-legal-notices-api-openapi.yml
- filename: companydata-dk-participants-api-openapi.yml
  format: yaml
  label: companydata.dk Participants API
  slug: companydata-dk-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-participants-api-openapi.yml
- filename: companydata-dk-production-units-api-openapi.yml
  format: yaml
  label: companydata.dk Production Units API
  slug: companydata-dk-production-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-production-units-api-openapi.yml
- filename: companydata-dk-properties-api-openapi.yml
  format: yaml
  label: companydata.dk Properties API
  slug: companydata-dk-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-properties-api-openapi.yml
- filename: companydata-dk-reference-data-api-openapi.yml
  format: yaml
  label: companydata.dk Reference Data API
  slug: companydata-dk-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-reference-data-api-openapi.yml
- filename: companydata-dk-screening-api-openapi.yml
  format: yaml
  label: companydata.dk Screening API
  slug: companydata-dk-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-screening-api-openapi.yml
- filename: companydata-dk-webhooks-api-openapi.yml
  format: yaml
  label: companydata.dk Webhooks API
  slug: companydata-dk-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-webhooks-api-openapi.yml
- filename: companydata-dk-working-lists-api-openapi.yml
  format: yaml
  label: companydata.dk Working Lists API
  slug: companydata-dk-working-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-dk/openapi/companydata-dk-working-lists-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: companydata.dk Authentication
name_suffix: Authentication
oauth_flows: []
overview: companydata.dk secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: companydata.dk
provider_slug: companydata-dk
scheme_count: 3
schemes:
- applies_to: REST API (api.companydata.dk/v1)
  description: 'API key authentication. Include your API key in the Authorization header: `Bearer sk_live_your_key`. Get your key at [companydata.dk](https://companydata.dk)'
  key_format: API keys start with `sk_live_` followed by a 32-character string. Keep your key secret and never expose it in client-side code.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/companydata-dk-openapi.yml
  - https://api.companydata.dk/v1/docs
  type: http
- applies_to: dawa.companydata.dk
  description: 'On dawa.companydata.dk a key is optional; from a server it is sent as `Authorization: Bearer sk_...` or `X-Api-Key: sk_...`; browser widgets put it in the path via the widget apiKey option.'
  name: DawaApiKey
  sources:
  - https://dawa.companydata.dk/
  type: apiKey
- applies_to: https://api.companydata.dk/mcp
  description: The MCP server at https://api.companydata.dk/mcp is connected via OAuth (log in to the companydata.dk account and click Allow); the page says it is built on MCP and OAuth 2.1, gets read-only access to company data, and access can be revoked from the account. No API keys are used.
  name: MCP OAuth
  sources:
  - https://companydata.dk/da/integrationer/mcp
  type: oauth2
slug: companydata-dk-authentication
source_filename: companydata-dk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://api.companydata.dk/v1/openapi.json\ndocs: https://api.companydata.dk/v1/docs\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key authentication. Include your API key in the Authorization header: `Bearer sk_live_your_key`. Get your key at [companydata.dk](https://companydata.dk)'\n  key_format: API keys start with `sk_live_` followed by a 32-character string. Keep your key secret and never expose it in client-side code.\n  applies_to: REST API (api.companydata.dk/v1)\n  sources:\n  - openapi/companydata-dk-openapi.yml\n  - https://api.companydata.dk/v1/docs\n- name: DawaApiKey\n  type: apiKey\n  description: 'On dawa.companydata.dk a key is optional; from a server it is sent as `Authorization: Bearer sk_...` or `X-Api-Key: sk_...`; browser widgets put it in the path via the widget apiKey option.'\n  applies_to: dawa.companydata.dk\n  sources:\n\
  \  - https://dawa.companydata.dk/\n- name: MCP OAuth\n  type: oauth2\n  description: The MCP server at https://api.companydata.dk/mcp is connected via OAuth (log in to the companydata.dk account and click Allow); the page says it is built on MCP and OAuth 2.1, gets read-only access to company data, and access can be revoked from the account. No API keys are used.\n  applies_to: https://api.companydata.dk/mcp\n  sources:\n  - https://companydata.dk/da/integrationer/mcp\nwebhook_signing:\n  algorithm: HMAC-SHA256\n  header: X-Companydata-Signature\n  delivery_id_header: X-Companydata-Delivery\n  note: The secret is returned only once, from POST /v1/webhooks.\n"
source_yaml_url: https://artifacts.apis.io/companydata-dk/authentication/companydata-dk-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company Data
- Business Registry
- CVR
- Denmark
- Credit Scoring
- Financial Statements
- Lead Generation
- MCP
- REST API
---
