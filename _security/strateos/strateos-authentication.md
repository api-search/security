---
api_key_in:
- header
auth_types:
- apiKey
- httpSignature
- http
description: ''
kind: authentication
layout: security
method: searched
name: Strateos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strateos secures its APIs with apiKey, httpSignature, and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Strateos
provider_slug: strateos
scheme_count: 3
schemes:
- description: Per-user email + API token retrieved from Developer Settings, sent to authenticate API requests (historically X-User-Email / X-User-Token headers).
  in: header
  name: apiKey
  source: https://developers.strateos.com/docs/developer-settings
  type: apiKey
- description: HTTP Message Signatures (draft-cavage httpsig). TxPy's StrateosSign signs requests over the (request-target), Date, and Host headers; write requests additionally sign Digest (SHA-256 of the body) and Content-Length, using an RSA secret.
  name: httpSignature
  scheme: signature
  signed_headers:
  - (request-target)
  - Date
  - Host
  - Digest
  - Content-Length
  source: https://github.com/strateos/transcriptic
  type: httpSignature
- description: Bearer token placed in the Authorization header (TxPy StrateosBearerAuth) for session/JWT-based access.
  name: bearer
  scheme: bearer
  source: https://github.com/strateos/transcriptic
  type: http
slug: strateos-authentication
source_filename: strateos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://developers.strateos.com/docs/developer-settings ;\n  https://github.com/strateos/transcriptic (transcriptic/auth.py)\ndocs: https://developers.strateos.com/docs/developer-settings\nsummary:\n  types:\n  - apiKey\n  - httpSignature\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    Strateos issues a per-user API Key from the Developer Settings tab of the user\n    administration page after developer access is requested. The official TxPy client\n    supports three request-auth mechanisms against the api_root (default\n    https://secure.strateos.com).\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-user email + API token retrieved from Developer Settings, sent to authenticate\n    API requests (historically X-User-Email / X-User-Token headers).\n  source: https://developers.strateos.com/docs/developer-settings\n- name: httpSignature\n  type: httpSignature\n  scheme: signature\n\
  \  description: >-\n    HTTP Message Signatures (draft-cavage httpsig). TxPy's StrateosSign signs requests\n    over the (request-target), Date, and Host headers; write requests additionally sign\n    Digest (SHA-256 of the body) and Content-Length, using an RSA secret.\n  signed_headers:\n  - (request-target)\n  - Date\n  - Host\n  - Digest\n  - Content-Length\n  source: https://github.com/strateos/transcriptic\n- name: bearer\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token placed in the Authorization header (TxPy StrateosBearerAuth) for\n    session/JWT-based access.\n  source: https://github.com/strateos/transcriptic\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strateos/refs/heads/main/authentication/strateos-authentication.yml
summary_line: apiKey/httpSignature/http · 3 schemes
tags:
- Company
- Life Sciences
- Laboratory Automation
- Robotics
- Cloud Lab
- Drug Discovery
- Biotechnology
- Autoprotocol
- JSON:API
- Research
---
