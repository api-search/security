---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Q2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Q2 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Q2
provider_slug: q2
scheme_count: 1
schemes:
- credentials:
    password: Secret
    username: API Key
  description: 'HTTP Basic Authentication via the Authorization header. The API Key is the Basic-auth username; the Secret is the Basic-auth password. The pair is combined and base64-encoded (e.g. Authorization: Basic base64(apiKey:secret)).'
  name: BasicAuth
  provisioning: API Key and Secret are issued via the Helix Admin site or by a Helix representative; sandbox and production credentials are distinct.
  scheme: basic
  type: http
slug: q2-authentication
source_filename: q2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.helix.q2.com/reference/authentication\ndocs: https://docs.helix.q2.com/reference/authentication\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic Authentication via the Authorization header. The API Key is the\n    Basic-auth username; the Secret is the Basic-auth password. The pair is\n    combined and base64-encoded (e.g. Authorization: Basic base64(apiKey:secret)).\n  credentials:\n    username: API Key\n    password: Secret\n  provisioning: API Key and Secret are issued via the Helix Admin site or by a Helix representative; sandbox and production credentials are distinct.\nnotes:\n- IP allowlisting is enforced in addition to Basic auth; requests must originate from a whitelisted (middleware/server) IP. End-user devices are not supported.\n- Versioning is bound to the API Key\
  \ (routes do not carry a version segment).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/q2/refs/heads/main/authentication/q2-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financial Services
- Banking
- Embedded Finance
- Banking as a Service
- FinTech
- Digital Banking
- Cards
- Payments
- ACH
- FDIC
---
