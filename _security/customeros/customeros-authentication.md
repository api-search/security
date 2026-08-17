---
api_key_in:
- header
api_specs:
- filename: customeros-customerbase-openapi.yml
  format: yaml
  label: CustomerOS REST API
  slug: customeros-customerbase-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-customerbase-openapi.yml
- filename: customeros-flow-api-openapi.yml
  format: yaml
  label: CustomerOS Flow API
  slug: customeros-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-flow-api-openapi.yml
- filename: customeros-graphql-api-openapi.yml
  format: yaml
  label: CustomerOS GraphQL API
  slug: customeros-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/openapi/customeros-graphql-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Customeros Authentication
name_suffix: Authentication
oauth_flows: []
overview: CustomerOS secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CustomerOS
provider_slug: customeros
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-CUSTOMER-OS-API-KEY
  sources:
  - openapi/customeros-billing-openapi.yml
  - openapi/customeros-customerbase-openapi.yml
  - openapi/customeros-domains-openapi.yml
  - openapi/customeros-enrich-openapi.yml
  - openapi/customeros-outreach-openapi.yml
  - openapi/customeros-verify-openapi.yml
  type: apiKey
- description: Per-tenant API key. The open-source customer-os-api validates an API key header and resolves the tenant before applying @hasRole / @hasTenant directives. Header name and exact auth flow depend on deployment; the documented customeros.ai cloud REST surface uses X-CUSTOMER-OS-API-KEY.
  in: header
  name: ApiKeyAuth
  parameter: X-Openline-API-KEY
  sources:
  - openapi/customeros-graphql-api-openapi.yml
  type: apiKey
slug: customeros-authentication
source_filename: customeros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/customeros-billing-openapi.yml, openapi/customeros-customerbase-openapi.yml,\n  openapi/customeros-domains-openapi.yml, openapi/customeros-enrich-openapi.yml, openapi/customeros-graphql-api-openapi.yml,\n  openapi/customeros-outreach-openapi.yml, openapi/customeros-verify-openapi.yml\ndocs_searched: true\ndocs_url: null\ndocs_note: >-\n  The CustomerOS documentation pages that used to describe API authentication —\n  docs.customeros.ai/api-overview and /api-descriptions — now return 404 and no longer appear in\n  the docs sitemap or llms.txt. The whole docs corpus was searched for \"api key\" through the\n  provider's own docs MCP filesystem and returned no match. So this profile stays DERIVED from the\n  published specs: the specs are now the only place CustomerOS documents API authentication at all.\n  docs.customeros.ai/security-and-compliance covers workspace SIGN-IN (magic link, Google/Microsoft\n  SSO, customer-supplied\
  \ OpenID Connect) — user identity, not API authorization.\nkey_issuance:\n  self_serve: false\n  note: >-\n    No key-issuance flow is published. Access to each REST endpoint group is granted per customer,\n    on request, by the CustomerOS team.\ndefect:\n  operation: POST /customerbase/v1/contacts/import\n  spec: openapi/customeros-customerbase-openapi.yml\n  issue: >-\n    Security requirement declares `ApiKeyAutl`, a typo for `ApiKeyAuth`, referencing a scheme that\n    is not defined in components.securitySchemes. Present in the provider's own published document.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-CUSTOMER-OS-API-KEY\n  sources:\n  - openapi/customeros-billing-openapi.yml\n  - openapi/customeros-customerbase-openapi.yml\n  - openapi/customeros-domains-openapi.yml\n  - openapi/customeros-enrich-openapi.yml\n  - openapi/customeros-outreach-openapi.yml\n  - openapi/customeros-verify-openapi.yml\n\
  - name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Openline-API-KEY\n  description: Per-tenant API key. The open-source customer-os-api validates an API key header\n    and resolves the tenant before applying @hasRole / @hasTenant directives. Header name and\n    exact auth flow depend on deployment; the documented customeros.ai cloud REST surface uses\n    X-CUSTOMER-OS-API-KEY.\n  sources:\n  - openapi/customeros-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customeros/refs/heads/main/authentication/customeros-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- CRM
- Revenue
- Go-To-Market
- Lead Intelligence
- Visitor Identification
- Attribution
- Email Verification
- Enrichment
- GraphQL
- Open Source
---
