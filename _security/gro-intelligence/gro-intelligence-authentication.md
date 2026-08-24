---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gro Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gro Intelligence secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gro Intelligence
provider_slug: gro-intelligence
scheme_count: 1
schemes:
- header_example: 'authorization: Bearer <GROAPI_TOKEN>'
  in: header
  name: bearerAuth
  note: 'Constructed identically in every endpoint helper in lib.py (get_allowed_units, get_available, list_available, lookup_single, lookup_batch, get_data_series, stream_data_series, get_top, get_source_ranking, get_available_timefrequency, get_data_points): `headers = {"authorization": "Bearer " + access_token}`. No other scheme appears anywhere in the client.'
  parameter_name: authorization
  scheme: bearer
  sources:
  - https://github.com/gro-intelligence/api-client/blob/development/groclient/lib.py
  token_type: opaque long-lived API token issued from the Gro web application
  type: http
slug: gro-intelligence-authentication
source_filename: gro-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://github.com/gro-intelligence/api-client/blob/development/groclient/lib.py\ndocs: https://gro.readthedocs.io/\nstatus: retired\nnote: >-\n  Gro Intelligence published no OpenAPI, so this profile is NOT derived from a\n  spec. It is read from the company's own first-party, MIT-licensed client\n  library on its live GitHub organization (gro-intelligence/api-client), where\n  every request builder sets the same header. The canonical auth documentation\n  (developers.gro-intelligence.com/authentication.html) is dead — the host does\n  not resolve — so gro.readthedocs.io is the only surviving published docs\n  mirror. The API itself is retired; this records how it worked.\nsummary:\n  types: [http]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: authorization\n  header_example: 'authorization: Bearer <GROAPI_TOKEN>'\n  token_type: opaque\
  \ long-lived API token issued from the Gro web application\n  sources:\n  - https://github.com/gro-intelligence/api-client/blob/development/groclient/lib.py\n  note: >-\n    Constructed identically in every endpoint helper in lib.py\n    (get_allowed_units, get_available, list_available, lookup_single,\n    lookup_batch, get_data_series, stream_data_series, get_top,\n    get_source_ranking, get_available_timefrequency, get_data_points):\n    `headers = {\"authorization\": \"Bearer \" + access_token}`. No other scheme\n    appears anywhere in the client.\ntoken_delivery:\n  env_var: GROAPI_TOKEN\n  note: >-\n    The official client and CLI read the token from the GROAPI_TOKEN\n    environment variable by default. Tokens were obtained from the Gro web\n    application (app.gro-intelligence.com), which no longer resolves — there is\n    no longer any way to obtain a credential.\nscopes: []\nscopes_note: >-\n  No OAuth surface and no scope model. Access was a single account-wide bearer\n \
  \ token, so scopes/ is correctly absent rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gro-intelligence/refs/heads/main/authentication/gro-intelligence-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Agriculture
- Climate
- Data
- Analytics
- Satellite Imagery
- Commodities
- Weather
- Food Security
- Time Series
- Defunct
---
