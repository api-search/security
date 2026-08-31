---
api_key_in:
- header
api_specs:
- filename: spectrumoutage-api-locations-api-openapi.yml
  format: yaml
  label: SpectrumOutage API Locations API
  slug: spectrumoutage-api-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectrumoutage-api/refs/heads/main/openapi/spectrumoutage-api-locations-api-openapi.yml
- filename: spectrumoutage-api-map-api-openapi.yml
  format: yaml
  label: SpectrumOutage API Map API
  slug: spectrumoutage-api-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectrumoutage-api/refs/heads/main/openapi/spectrumoutage-api-map-api-openapi.yml
- filename: spectrumoutage-api-reports-api-openapi.yml
  format: yaml
  label: SpectrumOutage API Reports API
  slug: spectrumoutage-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectrumoutage-api/refs/heads/main/openapi/spectrumoutage-api-reports-api-openapi.yml
- filename: spectrumoutage-api-stats-api-openapi.yml
  format: yaml
  label: SpectrumOutage API Stats API
  slug: spectrumoutage-api-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectrumoutage-api/refs/heads/main/openapi/spectrumoutage-api-stats-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Spectrumoutage Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpectrumOutage API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpectrumOutage API
provider_slug: spectrumoutage-api
scheme_count: 1
schemes:
- description: API key issued by SpectrumOutage.us. Request at usspectrumoutage@gmail.com
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spectrumoutage-api-openapi.yml
  - https://api.spectrumoutage.us
  type: http
slug: spectrumoutage-api-authentication
source_filename: spectrumoutage-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: openapi/spectrumoutage-api-openapi.yml\ndocs: https://api.spectrumoutage.us\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key issued by SpectrumOutage.us. Request at usspectrumoutage@gmail.com\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  sources:\n  - openapi/spectrumoutage-api-openapi.yml\n  - https://api.spectrumoutage.us\napplies_to: >-\n  Every operation. The requirement is declared once at the document root (`security: [{bearerAuth: []}]`)\n  and no operation overrides it, so there is no anonymous or partially-public endpoint in the v1 contract.\nissuance:\n  self_serve: false\n  channel: email\n  contact: usspectrumoutage@gmail.com\n  subject_line: API Key Request\n  requirements: state your use case and expected traffic\n  alternative: >-\n    A key can also be obtained by subscribing\
  \ to the RapidAPI listing\n    (https://rapidapi.com/usspectrumoutageus/api/spectrumoutage), where the BASIC plan is free with a\n    500,000 request/month hard cap.\n  note: >-\n    There is no developer signup, no key dashboard, and no rotation or revocation procedure documented.\n    Key lifecycle is entirely manual and out of band.\noauth:\n  supported: false\n  evidence: >-\n    No oauth2 or openIdConnect security scheme in the specification;\n    /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and\n    /.well-known/openid-configuration all return 404 on both spectrumoutage.us and api.spectrumoutage.us.\nscopes:\n  supported: false\n  note: >-\n    Bearer key auth with no scope model — a key carries the full surface including the POST /reports write\n    operation. No scopes artifact is emitted.\nfailure_modes:\n  - status: 401\n    condition: Authorization header absent\n    body: '{\"error\": {\"message\": \"Missing API key. Send Authorization: Bearer\
  \ <key>\"}}'\n  - status: 403\n    condition: key present but not recognised\n    body: '{\"error\": {\"message\": \"Invalid API key.\"}}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spectrumoutage-api/refs/heads/main/authentication/spectrumoutage-api-authentication.yml
summary_line: http · 1 scheme
tags:
- spectrum
- Outage
- internet
- tv
- phone
- Monitoring
- Status
- zip-code
- telecom
- isp
- network-status
- crowdsourced
---
