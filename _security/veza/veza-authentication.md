---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Veza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veza secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veza
provider_slug: veza
scheme_count: 1
schemes:
- description: 'API key issued from the Veza console, sent as `Authorization: Bearer <api_key>`. The oaaclient SDK constructs the connection as OAAClient(url=veza_url, token=veza_api_key); a missing URL or key is rejected client-side (MISSING_URL / MISSING_AUTH) before any request.'
  header: Authorization
  in: header
  name: VezaApiKey
  scheme: bearer
  sources:
  - github.com/veza/oaaclient-py/oaaclient/client.py
  type: http
slug: veza-authentication
source_filename: veza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.veza.com/ + github.com/veza/oaaclient-py (oaaclient/client.py)\ndocs: https://developer.veza.com/oaa/guide/getting-started.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Veza's Open Authorization API authenticates with a per-tenant API key\n    presented as a bearer token in the Authorization header. Each request is\n    made against the customer's own Veza tenant host (https://<tenant>.vezacloud.com).\n    No OAuth2 or OpenID Connect flow is exposed on the OAA REST surface.\nschemes:\n  - name: VezaApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    description: >-\n      API key issued from the Veza console, sent as `Authorization: Bearer <api_key>`.\n      The oaaclient SDK constructs the connection as OAAClient(url=veza_url, token=veza_api_key);\n      a missing URL or key is rejected client-side (MISSING_URL / MISSING_AUTH)\
  \ before any request.\n    sources: [github.com/veza/oaaclient-py/oaaclient/client.py]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veza/refs/heads/main/authentication/veza-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Identity Security
- Authorization
- Access Management
- Identity Governance
- API
---
