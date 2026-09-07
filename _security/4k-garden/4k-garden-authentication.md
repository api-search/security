---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 4k-garden-diebian-ai-openapi.json
  format: json
  label: Diebian AI Super-Resolution API
  slug: diebian-ai-super-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-diebian-ai-openapi.json
auth_types: []
description: Authentication profile for the Diebian AI super-resolution API. DERIVED from the published OpenAPI plus anonymous probes of the unauthenticated endpoints. The provider publishes no authentication documentation and no developer portal, so this profile is read from the contract's own shape rather than from a docs page.
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: 4K Garden Authentication
name_suffix: Authentication
oauth_flows: []
overview: 4K Garden declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: 4K Garden
provider_slug: 4k-garden
scheme_count: 0
schemes: []
slug: 4k-garden-authentication
source_filename: 4k-garden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/4k-garden-diebian-ai-openapi.json\nname: 4K Garden (Diebian AI) authentication profile\ndescription: >-\n  Authentication profile for the Diebian AI super-resolution API. DERIVED from the\n  published OpenAPI plus anonymous probes of the unauthenticated endpoints. The\n  provider publishes no authentication documentation and no developer portal, so this\n  profile is read from the contract's own shape rather than from a docs page.\napi: Diebian AI Super-Resolution API\nschemes: []\ndeclared_security_schemes: 0\nnotes: >-\n  The contract declares NO components.securitySchemes and no operation-level security[]\n  requirement, which is a springdoc default rather than a statement that the API is open.\n  The real mechanism is visible in the contract's own operations and responses.\nobserved_mechanism:\n  style: bearer-token\n  confidence: high\n  evidence:\n  - \"POST /api/auth/login (operationId loginUsingPOST) returns\
  \ ApiResponse«LoginResultVo», and LoginResultVo carries a `token` string alongside the `user` object.\"\n  - \"POST /api/auth/login-sms and POST /api/auth/register return the same LoginResultVo shape.\"\n  - \"GET /api/auth/me (operationId meUsingGET) is a current-principal endpoint, the canonical companion to a bearer token.\"\n  - \"All 63 operations declare 401 and 403 responses.\"\n  header: null\n  header_note: >-\n    The token header name is NOT stated anywhere in the contract or in any public\n    document, and is therefore not asserted here. An integrator would have to read it\n    off the web application's own network traffic.\ncredential_issuance:\n  self_service: partial\n  detail: >-\n    Registration exists (POST /api/auth/register) but GET /api/auth/register-config\n    returns {\"invite_code_required\": true}, so account creation is invite-gated.\n  probed: 'https://video-cn.fly4k.com/api/auth/register-config'\n  status: 200\nfactors:\n- type: password\n  operations: [loginUsingPOST,\
  \ resetPasswordUsingPOST, changePasswordUsingPUT]\n- type: sms-otp\n  operations: [loginSmsUsingPOST, smsCodeUsingPOST, verificationCodeUsingPOST]\nanonymous_endpoints:\n  note: Verified reachable with no credentials on 2026-09-05.\n  endpoints:\n  - path: /api/auth/health\n    status: 200\n  - path: /api/user/credit-rules\n    status: 200\n  - path: /api/user/productList\n    status: 200\n  - path: /api/user/enterprise-plans\n    status: 200\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\ngaps:\n- No securitySchemes declared in the contract.\n- No public authentication documentation of any kind.\n- Token transport header not published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/authentication/4k-garden-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Video
- Ultra High Definition
- Media and Entertainment
- Content Distribution
- Live Streaming
- Artificial Intelligence
- Video Super Resolution
- Virtual Reality
- China
---
