---
api_key_in: []
api_specs:
- filename: codametrix-components-api-openapi.yml
  format: yaml
  label: CodaMetrix Components API
  slug: codametrix-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-components-api-openapi.yml
- filename: codametrix-incidents-api-openapi.yml
  format: yaml
  label: CodaMetrix Incidents API
  slug: codametrix-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-incidents-api-openapi.yml
- filename: codametrix-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: CodaMetrix Scheduled Maintenances API
  slug: codametrix-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-scheduled-maintenances-api-openapi.yml
- filename: codametrix-status-api-openapi.yml
  format: yaml
  label: CodaMetrix Status API
  slug: codametrix-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-status-api-openapi.yml
- filename: codametrix-summary-api-openapi.yml
  format: yaml
  label: CodaMetrix Summary API
  slug: codametrix-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-summary-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Codametrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodaMetrix secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CodaMetrix
provider_slug: codametrix
scheme_count: 0
schemes: []
slug: codametrix-authentication
source_filename: codametrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://status.codametrix.com/api/ + live unauthenticated GETs of every /api/v2/ endpoint\ndocs: https://status.codametrix.com/api/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public_unauthenticated: true\nstatement: >-\n  The CodaMetrix Status API requires no authentication of any kind. Every endpoint under\n  https://status.codametrix.com/api/v2/ was fetched with no credentials, no API key and no Authorization\n  header and returned HTTP 200 with application/json. The documented cURL examples on CodaMetrix's own API\n  reference page carry no credential either. CORS is fully open (access-control-allow-origin: *), so the API\n  is callable directly from a browser or an agent with no key-provisioning step.\nschemes: []\nsurfaces:\n- name: CodaMetrix Status API\n  base_url: https://status.codametrix.com/api/v2/\n  auth: none\n  source: openapi/codametrix-status-openapi.yml\n  evidence: 8 of 8 endpoints\
  \ returned 200 unauthenticated on 2026-08-04\n- name: CMX CARE platform\n  auth: not public\n  note: >-\n    The CMX CARE autonomous coding platform is delivered through direct EHR integration (Epic Toolbox,\n    Cerner, Meditech, GE) under contract with each health system. There is no public developer portal, no\n    published developer API, no sign-up flow and therefore no public authentication model to document. This\n    is recorded as an honest absence, not a gap in the harvest.\n- name: Vanta Trust Center\n  url: https://trust.codametrix.com/\n  auth: signed-request\n  note: >-\n    The trust center's underlying GraphQL endpoint (POST https://trust.codametrix.com/graphql) rejects\n    anonymous calls with HTTP 400 \"Missing `signature` or `signedAt`\" — a Vanta-platform signed-request\n    scheme, not a CodaMetrix credential surface.\nnot_found:\n- {path: /.well-known/openid-configuration, host: www.codametrix.com, status: 404}\n- {path: /.well-known/oauth-authorization-server, host:\
  \ www.codametrix.com, status: 404}\n- {path: /.well-known/oauth-protected-resource, host: www.codametrix.com, status: 404}\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://status.codametrix.com/api/v2/summary.json', http_status: 200, auth_sent: none}\n  - {url: 'https://status.codametrix.com/api/v2/components.json', http_status: 200, auth_sent: none}\n  - {url: 'https://status.codametrix.com/api/', http_status: 200, note: documented cURL examples send no credential}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/authentication/codametrix-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- healthcare
- health-systems
- medical-coding
- autonomous-coding
- revenue-cycle-management
- clinical-documentation
- healthcare-ai
- machine-learning
- natural-language-processing
- ehr-integration
- status
---
