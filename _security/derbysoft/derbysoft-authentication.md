---
api_key_in: []
auth_types:
- http
- oauth2
description: 'DerbySoft Property Connector Integration API authentication. Access is granted with a Bearer token obtained via the OAuth 2.0 client-credentials pattern: the integrator obtains a Client ID (account_id) and Client Secret from DerbySoft (pms.service@derbysoft.net), Base64-encodes "client_id:client_secret" as HTTP Basic (RFC 7617) on the token endpoint, and receives an access token used as a Bearer token on all subsequent API calls. TLS 1.2+ over HTTPS is required.'
kind: authentication
layout: security
method: searched
name: Derbysoft Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: DerbySoft secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: DerbySoft
provider_slug: derbysoft
scheme_count: 2
schemes:
- description: HTTP Basic authentication per RFC 7617 used only against the token endpoint (POST /pcapigateway/account/token). Credentials are client_id (account_id) and client_secret joined with ":" and Base64-encoded.
  name: BasicTokenExchange
  response_fields:
  - accessToken
  - tokenType
  scheme: basic
  sources:
  - https://pc.knowledgebase.derbysoftsec.com/en/support/solutions/articles/70000663114-account
  token_endpoint: https://pcendpoint.derbysoftsec.com/pcapigateway/account/token
  type: http
- bearerFormat: opaque
  description: 'Bearer token presented on every API request as "Authorization: Bearer <accessToken>". Applying a new access token expires all previously issued tokens immediately; the PMS must call the token API at least once every 90 days to refresh the token.'
  name: BearerToken
  refresh_interval: at least once every 90 days
  scheme: bearer
  sources:
  - https://pc.knowledgebase.derbysoftsec.com/en/support/solutions/articles/70000157127-api-overview
  type: http
slug: derbysoft-authentication
source_filename: derbysoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://pc.knowledgebase.derbysoftsec.com/en/support/solutions/articles/70000663114-account\ndocs: https://pc.knowledgebase.derbysoftsec.com/en/support/solutions/articles/70000663114-account\ndescription: >-\n  DerbySoft Property Connector Integration API authentication. Access is granted\n  with a Bearer token obtained via the OAuth 2.0 client-credentials pattern: the\n  integrator obtains a Client ID (account_id) and Client Secret from DerbySoft\n  (pms.service@derbysoft.net), Base64-encodes \"client_id:client_secret\" as HTTP\n  Basic (RFC 7617) on the token endpoint, and receives an access token used as a\n  Bearer token on all subsequent API calls. TLS 1.2+ over HTTPS is required.\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicTokenExchange\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication per RFC 7617 used only\
  \ against the token endpoint\n    (POST /pcapigateway/account/token). Credentials are client_id (account_id)\n    and client_secret joined with \":\" and Base64-encoded.\n  token_endpoint: https://pcendpoint.derbysoftsec.com/pcapigateway/account/token\n  response_fields:\n  - accessToken\n  - tokenType\n  sources:\n  - https://pc.knowledgebase.derbysoftsec.com/en/support/solutions/articles/70000663114-account\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: >-\n    Bearer token presented on every API request as\n    \"Authorization: Bearer <accessToken>\". Applying a new access token expires\n    all previously issued tokens immediately; the PMS must call the token API at\n    least once every 90 days to refresh the token.\n  refresh_interval: at least once every 90 days\n  sources:\n  - https://pc.knowledgebase.derbysoftsec.com/en/support/solutions/articles/70000157127-api-overview\ncontacts:\n- pms.service@derbysoft.net\nnotes: >-\n  The Content\
  \ Distributor and Content Supplier (OTA 2016B) APIs use\n  supplier/distributor credentials issued by DerbySoft rather than the Property\n  Connector bearer token; their auth mechanics are not publicly documented on\n  the knowledge base.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/derbysoft/refs/heads/main/authentication/derbysoft-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- Travel
- Hospitality
- Hotels
- Distribution
- Connectivity
- Content
- Channel Management
- Travel Technology
---
