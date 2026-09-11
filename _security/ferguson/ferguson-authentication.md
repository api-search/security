---
anonymous_access: false
api_key_in: []
auth_types: []
description: Ferguson's Enterprise APIs are OAuth 2.0 protected. A partner registers on the Ferguson Developer Portal, is approved, creates a Developer/Team App, and receives a Key and Secret. The Key and Secret are base64-encoded into an HTTP Basic Authorization header on a call to the OAuth 2.0 token endpoint with grant_type=client_credentials; the returned access token is then presented on API calls as an Authorization header with the Bearer token type per RFC 6750. Ferguson's own portal documentation also covers the Authorization Code and Resource Owner Password Credentials (ROPC) grants. The token and API host names are published only inside the gated portal, so no endpoint URLs are recorded here.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ferguson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ferguson declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Ferguson
provider_slug: ferguson
scheme_count: 4
schemes:
- documented: true
  flow: clientCredentials
  id: oauth2-client-credentials
  note: Token endpoint URL is not published outside the approval-gated developer portal.
  source: https://developer.ferguson.com/blog/oauth-2-client-credentials-overview
  token_endpoint: null
  token_request_auth: http-basic (base64 of key:secret)
  token_request_params: grant_type=client_credentials
  type: oauth2
- authorization_endpoint: null
  documented: true
  flow: authorizationCode
  id: oauth2-authorization-code
  source: https://developer.ferguson.com/blog/oauth-2-authorization-code-grant
  token_endpoint: null
  type: oauth2
- documented: true
  flow: password
  id: oauth2-ropc
  note: Resource Owner Password Credentials grant, documented by Ferguson's portal. ROPC is deprecated in OAuth 2.1 and discouraged by RFC 9700 / the OAuth 2.0 Security BCP.
  source: https://developer.ferguson.com/blog/oauth-2-ropc-overview
  type: oauth2
- documented: true
  id: bearer-token
  note: '"REST API calls require an Authorization header using an access token with Bearer token type, as defined by the OAuth2 RFC6750 Bearer Token Usage document."'
  rfc: RFC 6750
  scheme: bearer
  source: https://developer.ferguson.com/get-started
  type: http
slug: ferguson-authentication
source_filename: ferguson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: >-\n  https://developer.ferguson.com/get-started,\n  https://developer.ferguson.com/blog/oauth-2-client-credentials-overview,\n  https://developer.ferguson.com/blog/oauth-2-ropc-overview,\n  https://developer.ferguson.com/blog/oauth-2-authorization-code-grant,\n  https://developer.ferguson.com/faq\nevidence_note: >-\n  developer.ferguson.com is a Backstage single-page application: the served HTML is a\n  6,575-byte shell and its backend (/api/catalog/*, /api/search/*) answers 401 \"Missing\n  credentials\" to anonymous requests, so these pages cannot be fetched as text by a\n  crawler. The statements below were read from the indexed public text of those exact\n  Ferguson URLs via web search on 2026-09-09. No credentialed access was used and no\n  values were inferred from any other provider.\ndescription: >-\n  Ferguson's Enterprise APIs are OAuth 2.0 protected. A partner registers on the Ferguson\n  Developer Portal, is approved,\
  \ creates a Developer/Team App, and receives a Key and\n  Secret. The Key and Secret are base64-encoded into an HTTP Basic Authorization header on\n  a call to the OAuth 2.0 token endpoint with grant_type=client_credentials; the returned\n  access token is then presented on API calls as an Authorization header with the Bearer\n  token type per RFC 6750. Ferguson's own portal documentation also covers the\n  Authorization Code and Resource Owner Password Credentials (ROPC) grants. The token and\n  API host names are published only inside the gated portal, so no endpoint URLs are\n  recorded here.\nschemes:\n  - id: oauth2-client-credentials\n    type: oauth2\n    flow: clientCredentials\n    documented: true\n    token_request_auth: http-basic (base64 of key:secret)\n    token_request_params: grant_type=client_credentials\n    token_endpoint: null\n    note: >-\n      Token endpoint URL is not published outside the approval-gated developer portal.\n    source: https://developer.ferguson.com/blog/oauth-2-client-credentials-overview\n\
  \  - id: oauth2-authorization-code\n    type: oauth2\n    flow: authorizationCode\n    documented: true\n    authorization_endpoint: null\n    token_endpoint: null\n    source: https://developer.ferguson.com/blog/oauth-2-authorization-code-grant\n  - id: oauth2-ropc\n    type: oauth2\n    flow: password\n    documented: true\n    note: >-\n      Resource Owner Password Credentials grant, documented by Ferguson's portal. ROPC is\n      deprecated in OAuth 2.1 and discouraged by RFC 9700 / the OAuth 2.0 Security BCP.\n    source: https://developer.ferguson.com/blog/oauth-2-ropc-overview\n  - id: bearer-token\n    type: http\n    scheme: bearer\n    documented: true\n    rfc: RFC 6750\n    note: >-\n      \"REST API calls require an Authorization header using an access token with Bearer\n      token type, as defined by the OAuth2 RFC6750 Bearer Token Usage document.\"\n    source: https://developer.ferguson.com/get-started\nonboarding:\n  self_service: false\n  gate: >-\n    Access is granted\
  \ only to organizations that complete Ferguson's partner review and\n    approval process; requests go to api.team@ferguson.com and approved requests are\n    backlogged and prioritized to business need.\n  contact: api.team@ferguson.com\n  docs: https://developer.ferguson.com/get-started\n  faq: https://developer.ferguson.com/faq\ngateway:\n  vendor: Google Apigee\n  evidence: >-\n    nonprod.developer.ferguson.com is an Apigee integrated developer portal — its Angular\n    bundle calls /portals/api/sites/:siteId/liveportal/* and /consumers/api/apps, the\n    Apigee portal API surface. The production portal has since moved to Backstage\n    (developer.ferguson.com serves a Backstage app shell with a backstage.io/config block\n    naming GitHub and Microsoft as its auth providers).\nscopes_published: false\nmtls: false\napi_keys_public: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferguson/refs/heads/main/authentication/ferguson-authentication.yml
summary_line: 4 schemes
tags:
- Distribution
- Plumbing
- HVAC
- Building Supplies
- Waterworks
- Pipe Valves Fittings
- Wholesale Distribution
- B2B
- Fortune 500
---
