---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Voi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Voi secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Voi
provider_slug: voi
scheme_count: 2
schemes:
- applies_to:
  - Voi MaaS Partner API
  description: MaaS Partner API (partners.voiapp.io/v1) endpoints are protected with token authentication using the X-Auth-Token request header, with a token issued by Voi when a partner signs up. Production keys are issued by Voi's engineering point of contact after development against staging is complete.
  in: header
  name: PartnerToken
  parameter: X-Auth-Token
  sources:
  - https://github.com/voiapp/partner-api-docs/blob/gh-pages/maas-pro.md
  type: apiKey
- applies_to:
  - Voi MDS Provider API
  - Voi GBFS API
  description: MDS and GBFS endpoints use OAuth 2.0 client credentials (two-legged OAuth, RFC 6749 section 4.4). POST basic-auth user:password with grant_type=client_credentials to the token endpoint; the response carries an access_token with expires_in 900 seconds and token_type bearer. The token is then required as Bearer authentication on all MDS and GBFS calls (docs also show an X-Auth-Token header form for GBFS requests).
  flows:
  - flow: clientCredentials
    scopes: []
    tokenUrl: https://mds.voiapp.io/token
  name: MDSClientCredentials
  sources:
  - https://github.com/voiapp/partner-api-docs/blob/gh-pages/maas-light.md
  type: oauth2
slug: voi-authentication
source_filename: voi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/voiapp/partner-api-docs/blob/gh-pages/maas-pro.md\ndocs: https://github.com/voiapp/partner-api-docs\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: PartnerToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: MaaS Partner API (partners.voiapp.io/v1) endpoints are protected with token\n    authentication using the X-Auth-Token request header, with a token issued by Voi when a\n    partner signs up. Production keys are issued by Voi's engineering point of contact after\n    development against staging is complete.\n  applies_to:\n  - Voi MaaS Partner API\n  sources:\n  - https://github.com/voiapp/partner-api-docs/blob/gh-pages/maas-pro.md\n- name: MDSClientCredentials\n  type: oauth2\n  description: MDS and GBFS endpoints use OAuth 2.0 client credentials (two-legged OAuth,\n    RFC 6749 section 4.4). POST\
  \ basic-auth user:password with grant_type=client_credentials\n    to the token endpoint; the response carries an access_token with expires_in 900 seconds\n    and token_type bearer. The token is then required as Bearer authentication on all MDS and\n    GBFS calls (docs also show an X-Auth-Token header form for GBFS requests).\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://mds.voiapp.io/token\n    scopes: []\n  applies_to:\n  - Voi MDS Provider API\n  - Voi GBFS API\n  sources:\n  - https://github.com/voiapp/partner-api-docs/blob/gh-pages/maas-light.md\nnotes:\n- Live probes on 2026-07-21 confirm the auth gates - partners.voiapp.io/v1/vehicles returns\n  401 without a token, mds.voiapp.io/v1/gbfs returns 401, and GET mds.voiapp.io/token returns\n  405 (POST-only), so the hosts and auth model documented above are still in service.\n- No OAuth scopes are documented for the client-credentials flow, so no scopes/ artifact is\n  produced for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voi/refs/heads/main/authentication/voi-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Micromobility
- E-Scooters
- E-Bikes
- Mobility-as-a-Service
- Transportation
- GBFS
- MDS
- Sweden
---
