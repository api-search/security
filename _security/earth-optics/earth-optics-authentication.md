---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Earth Optics Authentication
name_suffix: Authentication
oauth_flows: []
overview: EarthOptics secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EarthOptics
provider_slug: earth-optics
scheme_count: 2
schemes:
- bearerFormat: JWT
  evidence:
    challenge_header: 'www-authenticate: Bearer realm="api"'
    http_status: 401
    inference: The invalid-token response is the verbatim djangorestframework-simplejwt error shape, confirming JWT access/refresh tokens issued by Django REST Framework SimpleJWT. Token class "AccessToken" and token type "access" are reported by the server itself.
    invalid_token_body: '{"detail": "Given token not valid for any token type", "code": "token_not_valid", "messages": [{"token_class": "AccessToken", "token_type": "access", "message": "Token is invalid or expired"}]}'
    unauthenticated_body: '{"detail": "Authentication credentials were not provided."}'
  header: Authorization
  in: header
  name: bearerAuth
  realm: api
  scheme: bearer
  sources:
  - probe:https://api.earthoptics.com/api/schema/
  type: http
- evidence:
    challenge_header: 'vary: Accept, Cookie, Origin'
    confidence: medium
    inference: The Vary header includes Cookie, indicating Django session authentication is also enabled alongside Bearer — the pattern used by the app.earthoptics.com browser client.
  in: cookie
  name: sessionid
  sources:
  - probe:https://api.earthoptics.com/api/schema/
  type: apiKey
slug: earth-optics-authentication
source_filename: earth-optics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live unauthenticated HTTP probes of https://api.earthoptics.com\ndocs: null\ndocs_note: EarthOptics publishes no public authentication documentation; this profile\n  is observed from the API's own unauthenticated challenge responses, not from a spec\n  or a docs page.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  bearer_format: JWT\n  public_self_serve: false\n  gated: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  realm: api\n  in: header\n  header: Authorization\n  sources:\n  - probe:https://api.earthoptics.com/api/schema/\n  evidence:\n    challenge_header: 'www-authenticate: Bearer realm=\"api\"'\n    http_status: 401\n    unauthenticated_body: '{\"detail\": \"Authentication credentials were not provided.\"}'\n    invalid_token_body: '{\"detail\": \"Given token not valid for any token type\", \"code\":\n      \"token_not_valid\", \"messages\": [{\"token_class\"\
  : \"AccessToken\", \"token_type\":\n      \"access\", \"message\": \"Token is invalid or expired\"}]}'\n    inference: 'The invalid-token response is the verbatim djangorestframework-simplejwt\n      error shape, confirming JWT access/refresh tokens issued by Django REST Framework\n      SimpleJWT. Token class \"AccessToken\" and token type \"access\" are reported by\n      the server itself.'\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  name: sessionid\n  sources:\n  - probe:https://api.earthoptics.com/api/schema/\n  evidence:\n    challenge_header: 'vary: Accept, Cookie, Origin'\n    inference: The Vary header includes Cookie, indicating Django session authentication\n      is also enabled alongside Bearer — the pattern used by the app.earthoptics.com\n      browser client.\n    confidence: medium\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\ntoken_endpoint:\n  discovered: false\n  probed:\n  - path: /api/token/\n    status: 404\n  - path: /api/token/refresh/\n\
  \    status: 404\n  - path: /api/token/verify/\n    status: 404\n  - path: /api/auth/login/\n    status: 404\n  note: The SimpleJWT token endpoints are not mounted at any conventional public path;\n    credential exchange presumably happens on an internal route used by the SPA.\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\naccess:\n  self_serve_signup: false\n  developer_portal: false\n  documented: false\n  note: 'API access is available only to EarthOptics customers through the 360 PRO\n    application at app.earthoptics.com; there is no public API program, key issuance\n    flow, or published credential lifecycle.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earth-optics/refs/heads/main/authentication/earth-optics-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Agriculture
- AgTech
- Soil
- Soil Data
- Precision Agriculture
- Soil Carbon
- Carbon
- Sustainability
- Agronomy
- Geospatial
- Remote Sensing
- Soil Health
- Carbon Credits
---
