---
api_key_in: []
auth_types:
- bearer-token
description: Ladder's partner API is a client-side embedded integration, so its authentication model is a partner-minted user token rather than a provider-issued API key used from a browser. The public integration example shows the partner's own backend producing a user auth token which is passed to the LadderAPI constructor loaded in the page; the token identifies the end user on whose behalf the quoting/application flow is mounted. Ladder does not publish an OpenAPI document, an OAuth authorization server, or an OIDC discovery document (both /.well-known/oauth-authorization-server and /.well-known/openid-configuration return 404), and full reference credentials are issued only after a partner access request is approved. No scope surface is published, so no scopes/ artifact is asserted.
kind: authentication
layout: security
method: searched
name: Ladder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ladder secures its APIs with bearer-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ladder
provider_slug: ladder
scheme_count: 1
schemes:
- evidence: Published integration snippet on https://www.ladderlife.com/api — "// obtain user auth token from your server" then "const ladderAPI = new LadderAPI(userToken);"
  issued_by: partner backend
  location: client-side constructor argument
  name: userToken
  sources:
  - https://www.ladderlife.com/api
  type: bearer-token
slug: ladder-authentication
source_filename: ladder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.ladderlife.com/api\ndocs: https://www.ladderlife.com/api\ndescription: >-\n  Ladder's partner API is a client-side embedded integration, so its\n  authentication model is a partner-minted user token rather than a\n  provider-issued API key used from a browser. The public integration example\n  shows the partner's own backend producing a user auth token which is passed to\n  the LadderAPI constructor loaded in the page; the token identifies the end user\n  on whose behalf the quoting/application flow is mounted. Ladder does not\n  publish an OpenAPI document, an OAuth authorization server, or an OIDC\n  discovery document (both /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration return 404), and full reference credentials\n  are issued only after a partner access request is approved. No scope surface is\n  published, so no scopes/ artifact is asserted.\nsummary:\n  types:\n  - bearer-token\n\
  \  api_key_in: []\n  oauth2_flows: []\n  public_spec: false\n  access_model: partner-request\nschemes:\n- name: userToken\n  type: bearer-token\n  location: client-side constructor argument\n  issued_by: partner backend\n  evidence: >-\n    Published integration snippet on https://www.ladderlife.com/api —\n    \"// obtain user auth token from your server\" then\n    \"const ladderAPI = new LadderAPI(userToken);\"\n  sources:\n  - https://www.ladderlife.com/api\nnotes:\n- Reference documentation for server-side credentials is gated behind \"Request access\".\n- No published OAuth 2.0 or OpenID Connect surface as of this probe.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ladder/refs/heads/main/authentication/ladder-authentication.yml
summary_line: bearer-token · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Life Insurance
- Embedded Finance
- Embedded Insurance
- Financial Services
- Fintech
- Quoting
---
