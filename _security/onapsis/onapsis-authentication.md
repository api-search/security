---
api_key_in:
- header
auth_types:
- apiKey
- http
description: The Onapsis Platform API is authenticated with an API key generated in the Onapsis console UI, which is exchanged for a short-lived bearer access token used on subsequent GraphQL requests. Onapsis states the key-and-token model on its public API announcement; the exact token endpoint and header forms below are documented publicly by integration vendors that ship Onapsis connectors (Brinqa), not by an Onapsis reference page — the provider's own API reference sits behind the Customer Portal login. Provenance is recorded per field so the provider-published and third-party-documented parts stay distinguishable.
kind: authentication
layout: security
method: searched
name: Onapsis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onapsis secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Onapsis
provider_slug: onapsis
scheme_count: 2
schemes:
- in: header
  issued_by: Onapsis console UI (API key generation)
  name: onapsisApiKey
  parameter_name: Authorization
  source_type: third-party-documented
  sources:
  - https://docs.brinqa.com/docs/connectors/onapsis/
  type: apiKey
  used_for: token exchange only
  value_form: Basic <api_key>
- name: onapsisBearer
  scheme: bearer
  source_type: third-party-documented
  sources:
  - https://docs.brinqa.com/docs/connectors/onapsis/
  type: http
  used_for: all GraphQL API requests
slug: onapsis-authentication
source_filename: onapsis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://onapsis.com/blog/new-year-new-api-new-onapsis-api-custom-workflows-integrations/\ndocs: https://onapsis.com/customer-portal/\ndescription: >-\n  The Onapsis Platform API is authenticated with an API key generated in the\n  Onapsis console UI, which is exchanged for a short-lived bearer access token\n  used on subsequent GraphQL requests. Onapsis states the key-and-token model on\n  its public API announcement; the exact token endpoint and header forms below\n  are documented publicly by integration vendors that ship Onapsis connectors\n  (Brinqa), not by an Onapsis reference page — the provider's own API reference\n  sits behind the Customer Portal login. Provenance is recorded per field so the\n  provider-published and third-party-documented parts stay distinguishable.\nprovider_published: partial\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [basic, bearer]\n  oauth2_flows: []\n  oauth2:\
  \ false\n  openid_connect: false\n  mutual_tls: null\nschemes:\n- name: onapsisApiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  value_form: 'Basic <api_key>'\n  used_for: token exchange only\n  issued_by: Onapsis console UI (API key generation)\n  source_type: third-party-documented\n  sources:\n  - https://docs.brinqa.com/docs/connectors/onapsis/\n- name: onapsisBearer\n  type: http\n  scheme: bearer\n  used_for: all GraphQL API requests\n  source_type: third-party-documented\n  sources:\n  - https://docs.brinqa.com/docs/connectors/onapsis/\ntoken_exchange:\n  endpoint: POST https://{onapsis-console-host}/api/v1/token\n  request_auth: 'Authorization: Basic <api_key>'\n  response: access token\n  subsequent_auth: 'Authorization: Bearer <access_token>'\n  source_type: third-party-documented\n  source: https://docs.brinqa.com/docs/connectors/onapsis/\napi_surface:\n  protocol: GraphQL\n  path: POST /graphql\n  host_model: per-customer Onapsis console host (no shared\
  \ multi-tenant API host)\n  products_covered:\n  - Assess (full, at initial release)\n  - Comply (preliminary)\n  source: https://onapsis.com/blog/new-year-new-api-new-onapsis-api-custom-workflows-integrations/\ngaps:\n- The provider publishes no public API reference, no OpenAPI/GraphQL SDL, and no\n  anonymous introspection endpoint; the reference is inside the Customer Portal\n  (Salesforce Community) login.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n  is served (both 404), so token lifetime, refresh behavior and scopes could not\n  be verified.\nx-evidence:\n- url: https://onapsis.com/blog/new-year-new-api-new-onapsis-api-custom-workflows-integrations/\n  http_status: 200\n  kind: provider API announcement (GraphQL, API keys, access tokens)\n- url: https://docs.brinqa.com/docs/connectors/onapsis/\n  http_status: 200\n  kind: third-party connector documentation (token endpoint + header forms)\n- url: https://onapsis.com/.well-known/oauth-authorization-server\n\
  \  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onapsis/refs/heads/main/authentication/onapsis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Cybersecurity
- Application Security
- Vulnerability Management
- Compliance
- SAP
- ERP
- Threat Detection
- GraphQL
- Enterprise Software
---
