---
api_key_in: []
auth_types:
- oauth2
description: AstroPrint Cloud API authentication. The API is protected by OAuth 2.0. Apps are registered on the AstroPrint developer/development page to obtain a client_id and client_secret, then exchange them at the token endpoint. Both the client_credentials grant and the authorization_code grant are documented; the authorization_code (three-legged) flow is required for full access to a user's printers and designs, while client_credentials returns an empty dataset for user-scoped resources.
kind: authentication
layout: security
method: searched
name: 3Dagogo Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3DaGoGo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 3DaGoGo
provider_slug: 3dagogo
scheme_count: 1
schemes:
- description: OAuth 2.0. Register an app on the AstroPrint developer page to receive a client_id/client_secret plus the authorization and token URLs. Access tokens are sent as a Bearer token on API requests.
  docs: https://developer.astroprint.com/
  evidence:
  - https://api.astroprint.com/v2/printers returned HTTP 401 (auth required) at probe time
  - https://forum.astroprint.com/t/how-to-request-oauth-2-token-through-api/4384
  grants:
  - client_credentials
  - authorization_code
  name: oauth2
  scopes: []
  scopes_note: The developer documentation references scope selection during OAuth app setup, but AstroPrint does not publish a public enumerated scope reference, so no scope list is captured here (absence recorded, not fabricated).
  token_endpoint: https://api.astroprint.com/v2/token
  type: oauth2
slug: 3dagogo-authentication
source_filename: 3dagogo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  https://forum.astroprint.com/t/how-to-request-oauth-2-token-through-api/4384\n  and the AstroPrint developer portal (https://developer.astroprint.com).\n  Confirmed live: https://api.astroprint.com/v2/printers returns HTTP 401\n  without a token. No public OpenAPI is published, so this profile is captured\n  from the developer documentation rather than derived from a spec.\ndescription: >-\n  AstroPrint Cloud API authentication. The API is protected by OAuth 2.0. Apps\n  are registered on the AstroPrint developer/development page to obtain a\n  client_id and client_secret, then exchange them at the token endpoint. Both\n  the client_credentials grant and the authorization_code grant are documented;\n  the authorization_code (three-legged) flow is required for full access to a\n  user's printers and designs, while client_credentials returns an empty\n  dataset for user-scoped resources.\nsummary:\n  types:\n  - oauth2\n\
  base_url: https://api.astroprint.com/v2\nschemes:\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0. Register an app on the AstroPrint developer page to receive a\n    client_id/client_secret plus the authorization and token URLs. Access\n    tokens are sent as a Bearer token on API requests.\n  token_endpoint: https://api.astroprint.com/v2/token\n  grants:\n  - client_credentials\n  - authorization_code\n  scopes: []\n  scopes_note: >-\n    The developer documentation references scope selection during OAuth app\n    setup, but AstroPrint does not publish a public enumerated scope reference,\n    so no scope list is captured here (absence recorded, not fabricated).\n  docs: https://developer.astroprint.com/\n  evidence:\n  - https://api.astroprint.com/v2/printers returned HTTP 401 (auth required) at probe time\n  - https://forum.astroprint.com/t/how-to-request-oauth-2-token-through-api/4384\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3dagogo/refs/heads/main/authentication/3dagogo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- 3D Printing
- Cloud
- Manufacturing
- IoT
- Developer API
- OAuth
---
