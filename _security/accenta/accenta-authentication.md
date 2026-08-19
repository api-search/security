---
api_key_in: []
auth_types:
- cookie-session
description: ''
kind: authentication
layout: security
method: probed
name: Accenta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accenta secures its APIs with cookie-session across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Accenta
provider_slug: accenta
scheme_count: 1
schemes:
- description: 'Session established by the effiPilot login application and carried on subsequent /api/method/* calls as a cookie. Observed in the provider''s own login bundle, which issues every API call with withCredentials: true and resolves the current principal via GET /api/method/session.'
  evidence:
  - method_endpoint: GET https://app.accenta.ai/api/method/session
    note: session read used by the login app; requires the cookie
  - method_endpoint: GET https://app.accenta.ai/api/<tenant>/method/logout
    note: session teardown observed in the login app
  - method_endpoint: POST https://app.accenta.ai/api/method/lostLogin
    note: anonymous password-recovery method observed in the login app
  in: cookie
  name: effiPilotSession
  sources:
  - https://app.accenta.ai/login/main-JKA2JTKB.js
  type: apiKey
slug: accenta-authentication
source_filename: accenta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://app.accenta.ai/login/ (public Angular login application) + live probes of https://app.accenta.ai/api/\ndocs: https://app.accenta.ai/login/?redirectTo=api%2Fdoc\nnote: >-\n  There is no OpenAPI document to derive securitySchemes from, so this profile was established by\n  probing the effiPilot platform API and reading the provider's own publicly served login\n  application. The model is a server-side session cookie, not a bearer token or API key: the login\n  app calls the API with credentials attached to the request (withCredentials) and reads the session\n  from GET /api/method/session. Nothing in the public surface documents a machine-to-machine\n  credential — no API-key header, no OAuth 2.0 authorization server, no OIDC discovery document (see\n  well-known/accenta-well-known.yml, where every /.well-known/ path missed). Whether effiPilot\n  offers a token grant for programmatic clients can only be answered from the\
  \ gated API reference at\n  /api/doc.\nsummary:\n  types:\n  - cookie-session\n  api_key_in: []\n  oauth2_flows: []\n  machine_to_machine_credential_documented: false\nschemes:\n- name: effiPilotSession\n  type: apiKey\n  in: cookie\n  description: >-\n    Session established by the effiPilot login application and carried on subsequent /api/method/*\n    calls as a cookie. Observed in the provider's own login bundle, which issues every API call with\n    withCredentials: true and resolves the current principal via GET /api/method/session.\n  sources:\n  - https://app.accenta.ai/login/main-JKA2JTKB.js\n  evidence:\n  - method_endpoint: GET https://app.accenta.ai/api/method/session\n    note: session read used by the login app; requires the cookie\n  - method_endpoint: GET https://app.accenta.ai/api/<tenant>/method/logout\n    note: session teardown observed in the login app\n  - method_endpoint: POST https://app.accenta.ai/api/method/lostLogin\n    note: anonymous password-recovery method\
  \ observed in the login app\nanonymous_endpoints:\n- endpoint: GET https://app.accenta.ai/api/method/brandConf\n  status: 200\n  content_type: application/json\n  note: >-\n    Verified reachable with no credentials. Returns tenant branding, the Accenta SAS legal entity\n    block, consent/EULA versions and theme colours. This is the only unauthenticated method observed.\nobserved_response_headers:\n  access-control-allow-credentials: 'true'\n  access-control-allow-origin: http://localhost\n  referrer-policy: strict-origin-when-cross-origin\n  content-security-policy-report-only: present\n  x-powered-by: PHP/8.0.30\n  server: nginx/1.22.1\nx-evidence:\n- url: https://app.accenta.ai/api/method/brandConf\n  http_status: 200\n  fetched: '2026-08-17'\n- url: https://app.accenta.ai/api/doc\n  http_status: 404\n  fetched: '2026-08-17'\n  note: 'anonymous request returns {\"message\":\"Route not found\"}; the route is only served to a logged-in session'\n- url: https://app.accenta.ai/login/\n\
  \  http_status: 200\n  fetched: '2026-08-17'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accenta/refs/heads/main/authentication/accenta-authentication.yml
summary_line: cookie-session · 1 scheme
tags:
- Company
- Ai Data
- Energy
- Buildings
- Smart Buildings
- Building Management
- Geothermal
- Decarbonization
- Sustainability
- Energy Management
- Artificial Intelligence
- Real Estate
- IoT
- France
---
