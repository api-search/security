---
api_key_in:
- header
api_specs:
- filename: dragos-worldview-openapi-original.json
  format: json
  label: Dragos WorldView API
  slug: dragos-worldview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dragos/refs/heads/main/openapi/dragos-worldview-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dragos Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Dragos secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Dragos
provider_slug: dragos
scheme_count: 4
schemes:
- description: API Access Token
  in: header
  name: api_token
  parameter: API-Token
  sources:
  - openapi/dragos-worldview-openapi-original.json
  type: apiKey
- description: API Secret Key
  in: header
  name: api_secret
  parameter: API-Secret
  sources:
  - openapi/dragos-worldview-openapi-original.json
  type: apiKey
- description: NPE Token
  in: header
  name: npe_token
  parameter: Authorization
  sources:
  - openapi/dragos-worldview-openapi-original.json
  type: apiKey
- api: platform-sitestore
  description: Dragos Platform SiteStore v2 API accepts an OAuth 2.0 Bearer (JWT) access token (recommended, dynamic and expiring) or a static API key. Access is role-based (e.g. asset:read to read Asset data).
  name: platform_oauth2
  sources:
  - https://docs.ctpx.secureworks.com/integration/connectNetwork/dragos/
  type: oauth2
slug: dragos-authentication
source_filename: dragos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/dragos-worldview-openapi-original.json\ndocs: https://portal.dragos.com/api/v1/doc/index.html\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: API-Token\n  description: API Access Token\n  sources:\n  - openapi/dragos-worldview-openapi-original.json\n- name: api_secret\n  type: apiKey\n  in: header\n  parameter: API-Secret\n  description: API Secret Key\n  sources:\n  - openapi/dragos-worldview-openapi-original.json\n- name: npe_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: NPE Token\n  sources:\n  - openapi/dragos-worldview-openapi-original.json\n- name: platform_oauth2\n  type: oauth2\n  api: platform-sitestore\n  description: Dragos Platform SiteStore v2 API accepts an OAuth 2.0 Bearer (JWT) access token (recommended, dynamic and expiring) or a static\
  \ API key. Access is role-based (e.g. asset:read to read Asset data).\n  sources:\n  - https://docs.ctpx.secureworks.com/integration/connectNetwork/dragos/\napis:\n  worldview: apiKey headers (API-Token + API-Secret); NPE token via Authorization header\n  platform-sitestore: OAuth 2.0 Bearer JWT (recommended) or static API key, role-based (asset:read)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dragos/refs/heads/main/authentication/dragos-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Company
- Cybersecurity
- OT Security
- ICS
- Threat Intelligence
- Industrial Control Systems
- Indicators of Compromise
- STIX
- Vulnerability Management
- Security
---
