---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Awakens Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AWAKENS secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AWAKENS
provider_slug: awakens
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://genomelink.io/oauth/authorize
    flow: authorizationCode
    grant_type: authorization_code
    params:
    - client_id
    - client_secret
    - redirect_uri
    - scope
    response_type: code
    sources:
    - https://github.com/genomelink/genomelink-python/blob/master/genomelink/oauth.py
    - https://github.com/genomelink/genomelink-node/blob/master/src/OAuth.js
    tokenUrl: https://genomelink.io/oauth/token
  name: oauth2
  type: oauth2
- description: 'The issued OAuth access token is presented as an HTTP Bearer token (Authorization: Bearer <access_token>) on report requests. The enterprise reports endpoint presents the client secret as the Bearer credential.'
  name: bearer
  scheme: bearer
  sources:
  - https://github.com/genomelink/genomelink-python/blob/master/genomelink/resource/report.py
  type: http
slug: awakens-authentication
source_filename: awakens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/genomelink/genomelink-python\ndocs: https://genomelink.io/developers/\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  http_schemes: [bearer]\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://genomelink.io/oauth/authorize\n    tokenUrl: https://genomelink.io/oauth/token\n    grant_type: authorization_code\n    response_type: code\n    params: [client_id, client_secret, redirect_uri, scope]\n    sources:\n    - https://github.com/genomelink/genomelink-python/blob/master/genomelink/oauth.py\n    - https://github.com/genomelink/genomelink-node/blob/master/src/OAuth.js\n- name: bearer\n  type: http\n  scheme: bearer\n  description: >-\n    The issued OAuth access token is presented as an HTTP Bearer token\n    (Authorization: Bearer <access_token>) on report requests. The enterprise\n    reports endpoint\
  \ presents the client secret as the Bearer credential.\n  sources:\n  - https://github.com/genomelink/genomelink-python/blob/master/genomelink/resource/report.py\nnotes: >-\n  Derived and verified from AWAKENS' official first-party SDK source (Python and\n  Node.js). Standard OAuth 2.0 authorization-code flow against genomelink.io;\n  the API base is configurable via GENOMELINK_API_BASE and defaults to\n  https://genomelink.io. There is no apiKey scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awakens/refs/heads/main/authentication/awakens-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Genomics
- DNA
- Bioinformatics
- Health
- Consumer Genetics
- Ancestry
- OAuth
- Personal Genomics
---
