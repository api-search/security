---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: archer-daniels-midland-commodities-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Commodities API
  slug: archer-daniels-midland-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-commodities-api-openapi.yml
- filename: archer-daniels-midland-locations-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Locations API
  slug: archer-daniels-midland-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-locations-api-openapi.yml
- filename: archer-daniels-midland-products-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Products API
  slug: archer-daniels-midland-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-products-api-openapi.yml
auth_types:
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Archer Daniels Midland Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archer Daniels Midland secures its APIs with openIdConnect and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
scheme_count: 2
schemes:
- description: 'OpenID Connect / OAuth 2.0 authorization server published by ADM on www.adm.com. Issuer https://www.adm.com/; endpoints under /api/episerver/connect/. Grants: authorization_code, refresh_token, client_credentials. PKCE S256 supported. Client authentication: client_secret_basic or client_secret_post. This is the Optimizely (Episerver) CMS authorization server that fronts the adm.com website — it is genuinely first-party and machine-readable, but it is not a customer-facing API product.'
  method: probed
  name: openIdConnect
  observed_status: 200
  openIdConnectUrl: https://www.adm.com/.well-known/openid-configuration
  sources:
  - https://www.adm.com/.well-known/openid-configuration
  - https://www.adm.com/.well-known/oauth-authorization-server
  - well-known/archer-daniels-midland-openid-configuration.json
  type: openIdConnect
- description: 'API key header declared by the API-Evangelist-authored OpenAPI documents in this repo. NOT verified against ADM: the host these documents name (api.adm.com) has no DNS record.'
  in: header
  method: derived
  name: apiKey
  parameter: X-ADM-API-Key
  sources:
  - openapi/archer-daniels-midland-commodities-api-openapi.yml
  - openapi/archer-daniels-midland-locations-api-openapi.yml
  - openapi/archer-daniels-midland-products-api-openapi.yml
  type: apiKey
  verified: false
slug: archer-daniels-midland-authentication
source_filename: archer-daniels-midland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://www.adm.com/.well-known/openid-configuration (probed 2026-09-04) for the OIDC scheme;\n  openapi/archer-daniels-midland-commodities-api-openapi.yml,\n  openapi/archer-daniels-midland-locations-api-openapi.yml and\n  openapi/archer-daniels-midland-products-api-openapi.yml for the apiKey scheme\nnote: >-\n  ADM publishes no API authentication documentation — there is no developer portal, no API\n  reference, and the company's own llms.txt names no API. Read the two schemes below very\n  differently: the openIdConnect scheme was fetched from a live document ADM serves on its own\n  host; the apiKey scheme was DERIVED from OpenAPI documents that API Evangelist authored\n  (x-generated-from: documentation) against api.adm.com, a host that does not resolve. The header\n  name X-ADM-API-Key has never been observed on a live ADM response and should not be treated as a\n  provider-published fact.\nsummary:\n  types:\n  -\
  \ openIdConnect\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.adm.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect / OAuth 2.0 authorization server published by ADM on www.adm.com. Issuer\n    https://www.adm.com/; endpoints under /api/episerver/connect/. Grants: authorization_code,\n    refresh_token, client_credentials. PKCE S256 supported. Client authentication:\n    client_secret_basic or client_secret_post. This is the Optimizely (Episerver) CMS authorization\n    server that fronts the adm.com website — it is genuinely first-party and machine-readable, but\n    it is not a customer-facing API product.\n  method: probed\n  observed_status: 200\n  sources:\n  - https://www.adm.com/.well-known/openid-configuration\n  - https://www.adm.com/.well-known/oauth-authorization-server\n  - well-known/archer-daniels-midland-openid-configuration.json\n- name: apiKey\n  type: apiKey\n \
  \ in: header\n  parameter: X-ADM-API-Key\n  description: >-\n    API key header declared by the API-Evangelist-authored OpenAPI documents in this repo. NOT\n    verified against ADM: the host these documents name (api.adm.com) has no DNS record.\n  method: derived\n  verified: false\n  sources:\n  - openapi/archer-daniels-midland-commodities-api-openapi.yml\n  - openapi/archer-daniels-midland-locations-api-openapi.yml\n  - openapi/archer-daniels-midland-products-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/authentication/archer-daniels-midland-authentication.yml
summary_line: openIdConnect/apiKey · 2 schemes
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
---
