---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Wyatt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wyatt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Wyatt
provider_slug: wyatt
scheme_count: 2
schemes:
- applies_to: https://drforhair2024.cafe24api.com/api/mcp
  authorization_response_iss_parameter_supported: true
  authorization_url: https://drforhair2024.cafe24api.com/api/v2/oauth/authorize
  flow: authorizationCode
  id: oauth2_authorization_code
  pkce: true
  pkce_methods:
  - S256
  refresh_supported: true
  response_modes:
  - query
  response_types:
  - code
  revocation_url: https://drforhair2024.cafe24api.com/api/v2/oauth/revoke
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  token_url: https://drforhair2024.cafe24api.com/api/v2/oauth/token
  type: oauth2
- claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - jti
  - at_hash
  - auth_time
  - nonce
  - amr
  - mall.name
  - mall.email
  - mall.gender
  - mall.birthdate
  - mall.phone_number
  - mall.address
  id: openid_connect
  id_token_signing_algs:
  - RS256
  issuer: https://drforhair2024.cafe24api.com
  jwks_uri: https://drforhair2024.cafe24api.com/api/v2/.well-known/jwks.json
  openid_connect_url: https://drforhair.co.kr/.well-known/openid-configuration
  subject_types:
  - public
  type: openIdConnect
  userinfo_endpoint: https://drforhair2024.cafe24api.com/api/v2/customers/userinfo
slug: wyatt-authentication
source_filename: wyatt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://drforhair.co.kr/.well-known/openid-configuration\ndocs: https://developers.cafe24.com/app/front/app/develop/oauth\nnote: >-\n  Derived entirely from the OIDC discovery document Wyatt's own domain serves, plus the RFC 9728\n  protected-resource document. There is no OpenAPI to read securitySchemes from — Wyatt publishes\n  none. The authorization server is Cafe24's, running under Wyatt's tenant\n  (drforhair2024.cafe24api.com); service_documentation in the discovery document points at\n  developers.cafe24.com, which is Cafe24's developer portal, not Wyatt's.\noperator: cafe24\nschemes:\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://drforhair2024.cafe24api.com/api/v2/oauth/authorize\n  token_url: https://drforhair2024.cafe24api.com/api/v2/oauth/token\n  revocation_url: https://drforhair2024.cafe24api.com/api/v2/oauth/revoke\n  refresh_supported: true\n  pkce: true\n\
  \  pkce_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, none]\n  response_types: [code]\n  response_modes: [query]\n  authorization_response_iss_parameter_supported: true\n  applies_to: https://drforhair2024.cafe24api.com/api/mcp\n- id: openid_connect\n  type: openIdConnect\n  openid_connect_url: https://drforhair.co.kr/.well-known/openid-configuration\n  issuer: https://drforhair2024.cafe24api.com\n  jwks_uri: https://drforhair2024.cafe24api.com/api/v2/.well-known/jwks.json\n  userinfo_endpoint: https://drforhair2024.cafe24api.com/api/v2/customers/userinfo\n  subject_types: [public]\n  id_token_signing_algs: [RS256]\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - jti\n  - at_hash\n  - auth_time\n  - nonce\n  - amr\n  - mall.name\n  - mall.email\n  - mall.gender\n  - mall.birthdate\n  - mall.phone_number\n  - mall.address\nbearer:\n  methods_supported: [header]\n  source: https://drforhair.co.kr/.well-known/oauth-protected-resource\napi_keys: false\n\
  mutual_tls: false\nanonymous_surface:\n  description: >-\n    MCP initialize and tools/list succeed with no credential once a session is established; every\n    tools/call requires a bearer token. Anonymous discovery, authenticated action.\n  verified: probed\nx-evidence:\n  fetched: '2026-09-04'\n  openid_configuration_status: 200\n  oauth_authorization_server_status: 200\n  oauth_protected_resource_status: 200\n  jwks_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyatt/refs/heads/main/authentication/wyatt-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Beauty
- Personal Care
- Haircare
- Consumer Products
- E-Commerce
- Retail
- Agentic Commerce
- Model Context Protocol
- South Korea
---
