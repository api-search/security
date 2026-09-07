---
anonymous_access: false
api_key_in: []
auth_types: []
description: Willie's Reserve exposes two distinct authentication postures. The UCP/MCP commerce endpoint is anonymous — a tools/list call with no credentials returned the full tool set — while the customer-account surface is an OpenID Connect provider whose discovery document is served from the store's own domain and issued by Shopify on the store's behalf.
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Willie S Reserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Willie's Reserve declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Willie's Reserve
provider_slug: willie-s-reserve
scheme_count: 0
schemes: []
slug: willie-s-reserve-authentication
source_filename: willie-s-reserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://williesreserve.com/.well-known/openid-configuration\ndescription: >-\n  Willie's Reserve exposes two distinct authentication postures. The UCP/MCP commerce endpoint is\n  anonymous — a tools/list call with no credentials returned the full tool set — while the\n  customer-account surface is an OpenID Connect provider whose discovery document is served from\n  the store's own domain and issued by Shopify on the store's behalf.\nsurfaces:\n- name: UCP / MCP commerce endpoint\n  endpoint: https://williesreserve.com/api/ucp/mcp\n  scheme: none\n  type: anonymous\n  verified: probed\n  http_status: 200\n  note: >-\n    No Authorization header was sent and the server returned the full 13-tool manifest. Payment\n    still requires a buyer-approved payment instrument and explicit human approval at completion,\n    so anonymous discovery does not imply anonymous purchase.\n- name: Customer Accounts (OpenID Connect)\n  scheme: openIdConnect\n\
  \  type: oauth2\n  verified: probed\n  discovery:\n    openid_configuration: https://williesreserve.com/.well-known/openid-configuration\n    oauth_authorization_server: https://williesreserve.com/.well-known/oauth-authorization-server\n    status: 200\n  issuer: https://shopify.com/authentication/59591163950\n  authorization_endpoint: https://shopify.com/authentication/59591163950/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/59591163950/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/59591163950/logout\n  jwks_uri: https://shopify.com/authentication/59591163950/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  claims:\n\
  \  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  note: >-\n    The issuer is a Shopify-hosted authentication tenant keyed to this store's shop id\n    (59591163950); the discovery documents are served from williesreserve.com, which is why they\n    are recorded here rather than treated as a third party's.\nfiles:\n  openid_configuration: well-known/willie-s-reserve-openid-configuration.json\n  oauth_authorization_server: well-known/willie-s-reserve-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willie-s-reserve/refs/heads/main/authentication/willie-s-reserve-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Cannabis
- Consumer Products
- Retail
- Ecommerce
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
---
