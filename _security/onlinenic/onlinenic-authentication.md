---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile for the OnlineNIC Reseller API v4 (domain + SSL), transcribed from section 2.2 "Security Token" of the provider-published API 4.0.9 Reseller Guide (PDF). There is no OpenAPI securitySchemes block to derive from — OnlineNIC publishes no machine-readable contract — so every field below is read from the provider's own reference document and from a live unauthenticated probe of the API host.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Onlinenic Authentication
name_suffix: Authentication
oauth_flows: []
overview: OnlineNIC declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: OnlineNIC
provider_slug: onlinenic
scheme_count: 3
schemes:
- description: API key issued to the reseller. The guide states "This parameter is required for security Authentication. Partner can get this in Reseller Control panel." Sent as a POST body parameter, not as a header.
  id: apikey
  in: formData
  issued_via: Reseller Control Panel
  name: apikey
  required: true
  type: apiKey
- algorithm: md5
  components:
  - description: Reseller ID
    name: user
  - description: Reseller account password (hashed, never sent in the clear)
    name: password
  - description: Request timestamp; a request is valid for 10 minutes
    name: timestamp
  - description: Name of the method being called
    name: command
  description: Per-request security token. Token = MD5(user + MD5(password) + timestamp + command), lowercase 32-character MD5. Binds the request to the reseller id, the account password, the request timestamp and the command name.
  id: token
  in: formData
  name: token
  note: MD5 is used both for the password digest and for the request signature. It is a broken hash for signature purposes; HMAC-SHA256 would be the modern equivalent of this design. Recorded as an observation about the published scheme, not a vulnerability claim.
  required: true
  type: signed-request
- applies_to: live
  description: IP White List. "By adding IP to white list in Reseller control panel, the IP address will be whitelisted, and other IP address will be blocked from accessing API server. If the IP White list omitted, system will not set limitation with the IP address." Optional and off by default. Error 1021 ("Your IP does not exist in IP whitelist") is returned when it is configured and the caller is not on it.
  id: ip-allowlist
  note: The OTE test environment does not require IP allowlisting.
  required: false
  type: network
slug: onlinenic-authentication
source_filename: onlinenic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: OnlineNIC\nproviderId: onlinenic\ngenerated: '2026-09-17'\nmethod: searched\nsource: https://www.onlinenic.com/cp_english/template_api/download/Onlinenic_API_v4.0.9.2_Reseller_Guide.pdf\ndocs: https://www.onlinenic.com/cp_english/template_api/api_help.php\ndescription: >-\n  Authentication profile for the OnlineNIC Reseller API v4 (domain + SSL), transcribed from\n  section 2.2 \"Security Token\" of the provider-published API 4.0.9 Reseller Guide (PDF). There\n  is no OpenAPI securitySchemes block to derive from — OnlineNIC publishes no machine-readable\n  contract — so every field below is read from the provider's own reference document and from a\n  live unauthenticated probe of the API host.\nstyles:\n  - api-key\n  - signed-request\n  - ip-allowlist\nschemes:\n  - id: apikey\n    type: apiKey\n    in: formData\n    name: apikey\n    required: true\n    description: >-\n      API key issued\
  \ to the reseller. The guide states \"This parameter is required for security\n      Authentication. Partner can get this in Reseller Control panel.\" Sent as a POST body\n      parameter, not as a header.\n    issued_via: Reseller Control Panel\n  - id: token\n    type: signed-request\n    in: formData\n    name: token\n    required: true\n    algorithm: md5\n    description: >-\n      Per-request security token. Token = MD5(user + MD5(password) + timestamp + command),\n      lowercase 32-character MD5. Binds the request to the reseller id, the account password,\n      the request timestamp and the command name.\n    components:\n      - name: user\n        description: Reseller ID\n      - name: password\n        description: Reseller account password (hashed, never sent in the clear)\n      - name: timestamp\n        description: Request timestamp; a request is valid for 10 minutes\n      - name: command\n        description: Name of the method being called\n    note: >-\n      MD5\
  \ is used both for the password digest and for the request signature. It is a broken\n      hash for signature purposes; HMAC-SHA256 would be the modern equivalent of this design.\n      Recorded as an observation about the published scheme, not a vulnerability claim.\n  - id: ip-allowlist\n    type: network\n    required: false\n    description: >-\n      IP White List. \"By adding IP to white list in Reseller control panel, the IP address will\n      be whitelisted, and other IP address will be blocked from accessing API server. If the IP\n      White list omitted, system will not set limitation with the IP address.\" Optional and\n      off by default. Error 1021 (\"Your IP does not exist in IP whitelist\") is returned when it\n      is configured and the caller is not on it.\n    applies_to: live\n    note: The OTE test environment does not require IP allowlisting.\nrequired_parameters:\n  - user\n  - timestamp\n  - token\n  - apikey\ntransport:\n  protocol: https\n  method: POST\n\
  \  note: >-\n    \"API interface response to HTTPS call, and the request type must be POST.\" Credentials\n    travel in the POST body; there is no Authorization header and no bearer token.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  supported: false\n  note: >-\n    The API has no scope or permission model. A reseller API key carries the full command\n    surface for that reseller account, so scopes/ is deliberately not emitted.\nerrors:\n  - code: 1006\n    message: Authentication error.\n    meaning: Security token or password is wrong.\n  - code: 1020\n    message: Invalid API key.\n  - code: 1021\n    message: Your IP does not exist in IP whitelist.\n  - code: 1005\n    message: Object does not exist(user).\n    meaning: Invalid reseller ID.\nevidence:\n  - url: https://api.onlinenic.com/api4/ssl/index.php\n    method: GET\n    status: 200\n    body: '{\"code\":1001,\"msg\":\"Invalid request.\"}'\n    note: Live host answers the documented JSON envelope; GET\
  \ is rejected as the guide states.\n  - url: https://api.onlinenic.com/api4/domain/index.php?command=checkDomain\n    method: POST\n    status: 200\n    body: '{\"code\":1004,\"msg\":\"Required parameter missing(user).\"}'\n    note: Unauthenticated POST confirms `user` is the first required credential parameter.\nlegacy:\n  - api: OnlineNIC API 3.4 (deprecated)\n    transport: raw TCP socket, XML request/response\n    port: 30009\n    auth: chksum over category + action + params + cltrid, credentials in config\n    source: https://www.onlinenic.com/cp_english/template_api/download.php?f=sdk_php.zip\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onlinenic/refs/heads/main/authentication/onlinenic-authentication.yml
summary_line: 3 schemes
tags:
- Domains
- Domain Registration
- Registrar
- DNS
- SSL Certificates
- Certificates
- Reseller
- Hosting
- Security
---
