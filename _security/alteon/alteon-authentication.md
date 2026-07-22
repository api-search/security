---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Alteon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alteon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alteon
provider_slug: alteon
scheme_count: 1
schemes:
- description: HTTP Basic authentication with device username/password (base64-encoded), over HTTPS.
  docs: https://support.radware.com/app/answers/answer_view/a_id/16798/~/how-to-authenticate-the-alteon-rest-api
  name: basicAuth
  scheme: basic
  type: http
slug: alteon-authentication
source_filename: alteon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://support.radware.com/app/answers/answer_view/a_id/16798/~/how-to-authenticate-the-alteon-rest-api\ndocs: https://support.radware.com/app/answers/answer_view/a_id/16280/~/alteon-rest-api\nnotes: >-\n  The Alteon REST API is embedded in each Alteon device (accessed at\n  https://<device>/restdoc/, available from Alteon 34.0.4 / 33.5.8 / 33.0.12 and\n  above). There is no public multi-tenant OpenAPI to derive from, so this profile\n  is captured from Radware's documented auth model. Authentication is HTTP Basic\n  (username + password base64-encoded); Radware recommends restricting API access\n  over HTTPS.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with device username/password (base64-encoded), over HTTPS.\n  docs: https://support.radware.com/app/answers/answer_view/a_id/16798/~/how-to-authenticate-the-alteon-rest-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alteon/refs/heads/main/authentication/alteon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Infrastructure
- Application Delivery
- Load Balancing
- Application Delivery Controller
- Application Security
- Networking
- Radware
---
