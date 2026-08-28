---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Yazio Authentication
name_suffix: Authentication
oauth_flows: []
overview: YAZIO declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: YAZIO
provider_slug: yazio
scheme_count: 0
schemes: []
slug: yazio-authentication
source_filename: yazio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  live unauthenticated requests to https://yzapi.yazio.com, 2026-08-27\n  (GET /v15/user, GET /v14/user, POST /v15/oauth/token)\ndocumented: false\npointer_withheld: >-\n  No `type: Authentication` pointer is wired into apis.yml. The scoring check it\n  feeds is `authentication_documented`, and YAZIO documents none of this — every\n  field below was read off a live error response, not off a published auth page.\n  Wiring the pointer would credit YAZIO with documentation it has never shipped.\nsummary: >-\n  YAZIO's application backend is OAuth 2.0 with a resource-owner-password-credentials\n  grant that additionally requires a confidential client id and secret. The token\n  endpoint's own validation error, returned to an anonymous POST, names the four\n  required fields. Every resource endpoint probed answers 401 to an anonymous\n  request. None of this is published by YAZIO; it is observable only by calling the\n  host the\
  \ mobile apps call.\nsecurity_schemes:\n- name: oauth2_password\n  type: oauth2\n  flow: password\n  token_endpoint: https://yzapi.yazio.com/v15/oauth/token\n  content_type: application/x-www-form-urlencoded\n  required_parameters:\n  - username\n  - password\n  - client_id\n  - clientSecret\n  - grant_type\n  evidence:\n    url: https://yzapi.yazio.com/v15/oauth/token\n    method: POST\n    http_status: 400\n    body_excerpt: >-\n      [{\"property_path\":\"\",\"message\":\"Invalid client\"},{\"property_path\":\"username\",\n      \"message\":\"This value should not be blank.\"},{\"property_path\":\"password\",\n      \"message\":\"This value should not be blank.\"},{\"property_path\":\"clientSecret\",\n      \"message\":\"This value should not be blank.\"}]\n  note: >-\n    Client credentials are not issuable by any public YAZIO process — there is no\n    developer signup, no application registration and no client-id request form.\n    The credentials in circulation are the ones extracted\
  \ from the shipped mobile\n    apps by third parties.\n- name: bearer\n  type: http\n  scheme: bearer\n  applied_to: all probed resource endpoints\n  evidence:\n    url: https://yzapi.yazio.com/v15/user\n    method: GET\n    http_status: 401\nscopes: null\nscopes_note: >-\n  No scope surface was observable and none is documented. scopes/ is therefore not\n  emitted rather than emitted empty.\nversions_observed:\n- v14\n- v15\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yazio/refs/heads/main/authentication/yazio-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Health
- Digital Health
- Nutrition
- Calorie Tracking
- Weight Management
- Intermittent Fasting
- Fitness
- Consumer Health
- Mobile Applications
- Germany
---
