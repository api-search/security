---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Lotame Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lotame Solutions declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Lotame Solutions
provider_slug: lotame-solutions
scheme_count: 0
schemes: []
slug: lotame-solutions-authentication
source_filename: lotame-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://my.lotame.com/t/35h37my/admin-services-api + Panorama ID API docs\nname: Lotame Solutions Authentication Profile\napis:\n- name: Lotame Admin Services API\n  baseURL: https://api.lotame.com/2/\n  schemes:\n  - type: apiKey\n    in: header\n    scheme: lotame-token-pair\n    description: >-\n      Token-pair authentication using two custom headers sent on every request:\n      x-lotame-token (the token) and x-lotame-access (the access key). Both are\n      generated in the Spherical platform under Manage API Tokens > Create Token\n      Pair.\n    headers:\n    - x-lotame-token\n    - x-lotame-access\n    docs: https://my.lotame.com/t/35h37my/admin-services-api\n    notes: >-\n      User API tokens expire after 7 days by default and can be extended to 31\n      days on request. A separate Client API token type is available for\n      automated processes with up to one-year validity. HTTPS/TLS is required;\n      unauthorized\
  \ data access returns HTTP 403.\n- name: Panorama ID Server-Side API\n  baseURL: https://sid.crwdcntrl.net/sid\n  schemes:\n  - type: apiKey\n    in: body\n    scheme: client_id\n    description: >-\n      Requests are identified by a static integer client_id assigned by Lotame\n      and passed in the JSON request body. No bearer token or API key header is\n      required; per-request IAB TCF v2 or Lotame consent signaling is mandatory.\n    docs: https://my.lotame.com/t/60ykhkw/server-side-panorama-id-api-for-web\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lotame-solutions/refs/heads/main/authentication/lotame-solutions-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Data Management Platform
- Identity
- Advertising
- Marketing
- Audience Data
- Data Collaboration
- AdTech
---
