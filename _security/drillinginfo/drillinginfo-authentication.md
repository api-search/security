---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Drillinginfo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drillinginfo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Drillinginfo
provider_slug: drillinginfo
scheme_count: 2
schemes:
- access_token:
    format: bearer <access_token>
    header: Authorization
    scheme: bearer
    type: http
  credential:
    in: header
    name: secret_key
    provisioned_at: https://app.enverus.com/provisioning/directaccess
    type: apiKey
  name: DeveloperAPIv3
  sources:
  - docs
  token_endpoint: https://api.enverus.com/v3/direct-access/tokens
  version: v3
- access_token:
    format: bearer <access_token>
    header: Authorization
    scheme: bearer
    type: http
  credential:
    fields:
    - client_id
    - client_secret
    - api_key
    type: oauth-client-credentials
  name: DirectAccessV2
  sources:
  - docs
  token_endpoint: https://di-api.drillinginfo.com/v2/direct-access/tokens
  version: v2
slug: drillinginfo-authentication
source_filename: drillinginfo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.enverus.com/direct/#/api/explorer/v3/gettingStarted\ndocs: https://app.enverus.com/provisioning/directaccess\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  model: token-exchange\n  note: >-\n    A long-lived credential (v3 secret key, or v2 client_id/client_secret + API\n    key) is exchanged at the /tokens endpoint for a short-lived bearer access\n    token that is sent on the Authorization header for dataset requests. The\n    official client refreshes the token automatically on 401.\nschemes:\n- name: DeveloperAPIv3\n  version: v3\n  token_endpoint: https://api.enverus.com/v3/direct-access/tokens\n  credential:\n    type: apiKey\n    in: header\n    name: secret_key\n    provisioned_at: https://app.enverus.com/provisioning/directaccess\n  access_token:\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: bearer <access_token>\n  sources: [docs]\n\
  - name: DirectAccessV2\n  version: v2\n  token_endpoint: https://di-api.drillinginfo.com/v2/direct-access/tokens\n  credential:\n    type: oauth-client-credentials\n    fields: [client_id, client_secret, api_key]\n  access_token:\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: bearer <access_token>\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillinginfo/refs/heads/main/authentication/drillinginfo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Energy
- Oil and Gas
- Data
- Analytics
- Geospatial
- Developer API
- Well Data
- Production Data
- Energy Intelligence
---
