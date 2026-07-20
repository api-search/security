---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kuaishou Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kuaishou declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Kuaishou
provider_slug: kuaishou
scheme_count: 0
schemes: []
slug: kuaishou-authentication
source_filename: kuaishou-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://open.kuaishou.com/oauth2/authorize (HTTP 200), https://open.kuaishou.com/oauth2/access_token (HTTP 200, JSON)\nnotes: >-\n  Verified by live HTTP probe on 2026-07-19. The Kuaishou Open Platform developer documentation is served\n  as a JavaScript single-page application and its written scope/permission reference is gated behind\n  developer registration, so only the endpoints and behaviours observed directly on the wire are recorded\n  here. No scope list is asserted because none could be verified without an approved developer account.\napis:\n- api: kuaishou:open-platform\n  base_url: https://open.kuaishou.com/openapi\n  schemes:\n  - id: kuaishou_oauth2\n    type: oauth2\n    flow: authorization_code\n    authorization_url: https://open.kuaishou.com/oauth2/authorize\n    token_url: https://open.kuaishou.com/oauth2/access_token\n    evidence:\n      authorization_endpoint_status: 200\n      authorization_endpoint_content_type:\
  \ text/html\n      authorization_endpoint_behaviour: >-\n        Returns the Kuaishou Open Platform authorization / login interface, consistent with an OAuth 2.0\n        authorization-code front channel.\n      token_endpoint_status: 200\n      token_endpoint_content_type: application/json;charset=UTF-8\n      token_endpoint_unparameterised_response: >-\n        {\"result\":100200100,\"error\":\"invalid_request\",\"error_msg\":\"请求参数错误，请检查参数是否合法\"}\n      token_endpoint_note: >-\n        The token endpoint answers an unparameterised request with the OAuth 2.0 `invalid_request` error\n        identifier wrapped in Kuaishou's own result/error_msg envelope.\n    scopes_documented: unverified\n    scopes_source: null\n- api: kuaishou:kwai-for-business\n  base_url: https://developers.kwai.com/rest/n/mapi\n  schemes:\n  - id: kwai_business_unverified\n    type: unverified\n    evidence:\n      probe_status: 404\n      probe_content_type: application/json;charset=UTF-8\n      probe_response:\
  \ >-\n        {\"timestamp\":\"...\",\"status\":404,\"error\":\"Not Found\",\"message\":\"No message available\",\n        \"path\":\"/rest/n/mapi/...\"}\n      note: >-\n        The host routes /rest/n/mapi/* through a JSON application server, but no authorization or token\n        endpoint could be confirmed without an approved Kwai for Business advertiser account. No scheme\n        is asserted.\ngaps:\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server document is published\n  on any Kuaishou or Kwai host (all requests are absorbed by the SPA catch-all; see\n  well-known/kuaishou-well-known.yml).\n- No public OAuth scope / permission reference could be retrieved; scopes/ is intentionally not produced\n  rather than fabricated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuaishou/refs/heads/main/authentication/kuaishou-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Consumer
- Social
- Video
- Short Video
- Live Streaming
- Advertising
- Marketing
- Social Media
- Content
- China
---
