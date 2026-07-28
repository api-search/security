---
api_key_in: []
api_specs:
- filename: utilita-status-openapi.yml
  format: yaml
  label: Utilita Status API
  slug: utilita-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/openapi/utilita-status-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: derived
name: Utilita Authentication
name_suffix: Authentication
oauth_flows: []
overview: Utilita secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Utilita
provider_slug: utilita
scheme_count: 1
schemes:
- applies_to: Utilita Status API (https://status.utilita.co.uk/api/v2)
  detail: 'All eight operations were retrieved with no credentials and returned HTTP 200. The spec declares `security: []` at the document and operation level to state this explicitly.'
  name: none
  sources:
  - openapi/utilita-status-openapi.yml
  type: none
slug: utilita-authentication
source_filename: utilita-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/utilita-status-openapi.yml + anonymous probes of Utilita hosts on 2026-07-27\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  detail: >-\n    Utilita's one public API — the Utilita Status API — is fully anonymous. Every other Utilita\n    surface is a human login, not a documented API authentication scheme. There is no developer\n    credential of any kind to obtain: no API keys, no OAuth 2.0, no OpenID Connect discovery, no\n    mTLS, no client-credentials flow.\nschemes:\n- name: none\n  type: none\n  applies_to: Utilita Status API (https://status.utilita.co.uk/api/v2)\n  sources: [openapi/utilita-status-openapi.yml]\n  detail: >-\n    All eight operations were retrieved with no credentials and returned HTTP 200. The spec declares\n    `security: []` at the document and operation level to state this explicitly.\nhuman_authentication_surfaces:\n- surface: My Utilita customer portal\n  url: https://my.utilita.co.uk/login\n\
  \  model: server-side session cookies (XSRF-TOKEN + myutilita_session), Imperva/Incapsula in front\n  api_credential: false\n- surface: Utilita broker / partner portals\n  urls: [https://uportal.utilita.co.uk/login, https://whqapi.utilita.co.uk/login, https://broker.utilita.co.uk/]\n  model: private login pages behind a WAF; no published authentication contract\n  api_credential: false\ndiscovery_probes:\n  date: '2026-07-27'\n  results:\n  - {url: 'https://utilita.co.uk/.well-known/openid-configuration', status: 404}\n  - {url: 'https://my.utilita.co.uk/.well-known/openid-configuration', status: 404}\n  - {url: 'https://uportal.utilita.co.uk/.well-known/openid-configuration', status: 404}\n  - {url: 'https://whqapi.utilita.co.uk/.well-known/openid-configuration', status: 404}\n  - {url: 'https://join.utilita.co.uk/.well-known/openid-configuration', status: 403, note: blocked by Imperva WAF}\n  - {url: 'https://utilita.co.uk/.well-known/oauth-authorization-server', status: 404}\n  - {url:\
  \ 'https://my.utilita.co.uk/.well-known/oauth-authorization-server', status: 404}\nnotes: >-\n  Third parties who need GB smart-meter data with consumer consent authenticate to the Smart DCC as\n  a Smart Energy Code \"Other User\", not to Utilita. That is a regulated accession process with its\n  own security assurance regime — it is not a Utilita credential and is out of scope for this file.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/authentication/utilita-authentication.yml
summary_line: none · 1 scheme
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Prepayment
- Energy Retail
- Status
- Operational Transparency
---
