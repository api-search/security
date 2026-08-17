---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Sendible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sendible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sendible
provider_slug: sendible
scheme_count: 1
schemes:
- description: 'Every path under https://api.sendible.com/api/v1 answers HTTP 401 with the response header `WWW-Authenticate: Basic realm="Application"` and the body `HTTP Basic: Access denied.` — including paths that do not exist, so the challenge is emitted by the edge before routing. This is an OBSERVED runtime fact, not a documented contract.'
  name: basicAuth
  realm: Application
  scheme: basic
  sources:
  - 'probe: https://api.sendible.com/api/v1/services.json'
  type: http
slug: sendible-authentication
source_filename: sendible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: 'live unauthenticated GET https://api.sendible.com/api/v1/services.json'\ndocs: null\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  publicly_documented: false\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    realm: Application\n    description: >-\n      Every path under https://api.sendible.com/api/v1 answers HTTP 401 with the\n      response header `WWW-Authenticate: Basic realm=\"Application\"` and the body\n      `HTTP Basic: Access denied.` — including paths that do not exist, so the\n      challenge is emitted by the edge before routing. This is an OBSERVED\n      runtime fact, not a documented contract.\n    sources: ['probe: https://api.sendible.com/api/v1/services.json']\nevidence:\n  - {url: 'https://api.sendible.com/api/v1', http_status: 401, www_authenticate: 'Basic realm=\"Application\"'}\n  - {url: 'https://api.sendible.com/api/v1/services.json',\
  \ http_status: 401, body: 'HTTP Basic: Access denied.'}\n  - {url: 'https://api.sendible.com/api/v1/mentions.json', http_status: 401, body: 'HTTP Basic: Access denied.'}\n  - {url: 'https://api.sendible.com/api/v1/openapi.json', http_status: 401, body: 'HTTP Basic: Access denied.'}\nnote: >-\n  NO `Authentication` pointer is emitted in apis.yml for this file, deliberately.\n  The scoring check it feeds is `authentication_documented`, and Sendible\n  publishes no authentication documentation anywhere on a first-party surface:\n  developers.sendible.com is retired (301 to the marketing home page) and the\n  Zendesk help centre carries no API article — the former \"How do I set up\n  services for my clients via the API?\" article (id 208053026) now returns 404\n  from the help-centre API. Credentials (application id, API key, shared key/iv)\n  are issued only from inside a signed-in Sendible account. This artifact\n  records what we could observe from outside; it must not be read as the\n\
  \  provider documenting their auth model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendible/refs/heads/main/authentication/sendible-authentication.yml
summary_line: http · 1 scheme
tags:
- Social Media
- Social Media Management
- Agencies
- Scheduling
- Analytics
- Monitoring
---
