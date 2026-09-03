---
api_key_in: []
api_specs:
- filename: hanyang-repository-oai-pmh-openapi.yml
  format: yaml
  label: Repository at Hanyang University — OAI-PMH
  slug: repository-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hanyang/refs/heads/main/openapi/hanyang-repository-oai-pmh-openapi.yml
auth_types: []
description: 'Authentication model for the Hanyang University Open API, derived from the university''s own published Korean-language documentation at /develop/auths.page and /develop/guide.page (both HTTP 200, publicly readable without login on 2026-09-01). Hanyang classifies its Open APIs as "Public" (no personal data, key only) and "Private" (personal data, end-user OAuth consent required). No endpoint was exercised: the API catalogue itself is behind developer registration, so nothing below was confirmed by calling it.'
kind: authentication
layout: security
method: derived
name: Hanyang Open Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hanyang University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Hanyang University
provider_slug: hanyang
scheme_count: 0
schemes: []
slug: hanyang-open-api-authentication
source_filename: hanyang-open-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Hanyang University\nproviderId: hanyang\nname: Hanyang University Open API — OAuth 2.0 authentication\ngenerated: '2026-09-01'\nmethod: derived\nsource: https://api.hanyang.ac.kr/develop/auths.page\nx-operator: institution\nx-operator-evidence: >-\n  api.hanyang.ac.kr is under the institution's own registrable domain hanyang.ac.kr;\n  the authorization and token endpoints are on that same host and the terms of service\n  name Hanyang University as the service operator.\ndescription: >-\n  Authentication model for the Hanyang University Open API, derived from the\n  university's own published Korean-language documentation at\n  /develop/auths.page and /develop/guide.page (both HTTP 200, publicly readable\n  without login on 2026-09-01). Hanyang classifies its Open APIs as \"Public\"\n  (no personal data, key only) and \"Private\" (personal data, end-user OAuth\n  consent required). No endpoint\
  \ was exercised: the API catalogue itself is\n  behind developer registration, so nothing below was confirmed by calling it.\ntags:\n  - Authentication\n  - OAuth\n  - Education\n  - Higher Education\n  - University\nauthenticationTypes:\n  - type: OAuth 2.0\n    description: >-\n      Adopted for access to protected resources (Private APIs). Access is granted\n      only after the end user logs in and consents to the scopes the app requests;\n      refusal returns an authentication failure from Hanyang's authorization server.\n    flows:\n      - name: authorization_code\n        label: Web app — server-side flow\n        authorizationEndpoint: https://api.hanyang.ac.kr/oauth/authorize\n        tokenEndpoint: https://api.hanyang.ac.kr/oauth/token\n        parameters:\n          - name: client_id\n            required: true\n            description: Client ID issued after the app is approved.\n          - name: response_type\n            required: true\n            value: code\n      \
  \    - name: redirect_uri\n            required: true\n            description: Redirect URI registered with the app.\n          - name: scope\n            required: true\n            description: >-\n              Comma-separated list of the numeric API ids the app is registered to\n              use (documented example \"1,2,3,4\"). Scope is an API identifier list,\n              not a named permission string.\n          - name: client_secret\n            required: true\n            appliesTo: token request\n          - name: grant_type\n            required: true\n            value: authorization_code\n      - name: implicit\n        label: JavaScript app — client-side flow\n        authorizationEndpoint: https://api.hanyang.ac.kr/oauth/authorize\n        description: >-\n          Documented for JavaScript apps; the access token is returned directly to\n          the client rather than exchanged from an authorization code.\n  - type: API key\n    description: >-\n      Every Open API\
  \ call, Public or Private, requires a key issued by the Developer\n      Center. CLIENT ID and CLIENT SECRET are issued only after an administrator\n      approves the registered app; CLIENT SECRET can be reissued from My App.\n    keyIssuance:\n      registration: https://api.hanyang.ac.kr/member/join_step01.page\n      appRegistration: https://api.hanyang.ac.kr/develop/guide.page\n      approval: manual administrator approval required\n      steps:\n        - Accept the Open API terms of service.\n        - Register the app (name, description, service type Android/iOS/Web, redirect URL).\n        - Select the APIs the app will call.\n        - Request administrator approval.\n        - Collect the issued CLIENT ID and CLIENT SECRET.\nrequestSigning:\n  parameterEncryption: >-\n    The published error table carries RequiredSwapKeyException, CipherNotFoundException\n    and DecodeFailedException, indicating that at least some parameters are transmitted\n    encrypted and require a valid\
  \ decryption (\"swap\") key. The key exchange mechanism\n    is not documented on the public pages.\nipRestrictions: >-\n  UnAuthorizedAccessException (\"허가되지 않은 IP 입니다\", HTTP 401) indicates per-app IP\n  allow-listing is enforced.\nnotes: >-\n  Derived from documentation only. The API catalogue at /api/search.page renders an\n  empty template to anonymous visitors, and /develop/console.page, /notice/list.page\n  and /board/list.page all return the login form, so no endpoint list, scope list or\n  live token exchange could be verified.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanyang/refs/heads/main/authentication/hanyang-open-api-authentication.yml
summary_line: 0 schemes
tags:
- Authentication
- OAuth
- Education
- Higher Education
- University
---
