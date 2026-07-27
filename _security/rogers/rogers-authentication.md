---
api_key_in:
- password
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rogers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rogers Communications secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rogers Communications
provider_slug: rogers
scheme_count: 3
schemes:
- credential: username + API key, colon-joined and Base64 encoded in the Authorization header
  evidence:
  - body: '{"errorMessage":"Full authentication is required to access this resource"}'
    date: '2026-07-25'
    header: 'WWW-Authenticate: Basic realm="Jasper"'
    kind: live-probe
    request: GET https://restapi1.jasper.com/rws/api/v1/devices
    status: 401
  - kind: docs
    quote: '"concatenate the user name and API key (separated by a colon) ... encrypt the resulting string using Base64 ... set the authorization header value to ''Basic'' followed by the encoded string."'
    url: https://developer.cisco.com/docs/control-center/getting-started/
  interface: REST
  name: basicAuth
  realm: Jasper
  scheme: basic
  transport: HTTPS only (the REST APIs do not support plain HTTP)
  type: http
- credential: platform license key
  interface: SOAP
  name: licenseKey
  note: Cisco IoT Control Center SOAP API authentication. Rogers lists "Access to applicable REST and SOAP APIs" as a Rogers Control Centre Advantage tier feature. The SOAP servlet mount is live on the Rogers tenant host — every path under https://rogers.jasper.com/ws/service/ answers HTTP 405 to a GET, consistent with a POST-only SOAP endpoint (a nonexistent service name answers 405 as well, so individual service names could not be enumerated anonymously).
  type: apiKey
- credential: shared secret used to sign and validate inbound callback requests
  interface: PUSH (callbacks)
  name: sharedSecret
  note: Cisco IoT Control Center PUSH API callbacks. Cisco documents that "for the PUSH API it is necessary to configure a shared secret to validate the signature of incoming requests." Rogers publishes no event catalog of its own.
  type: signature
slug: rogers-authentication
source_filename: rogers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://developer.cisco.com/docs/control-center/getting-started/\ndocs: https://developer.cisco.com/docs/control-center/rest-api-troubleshooting-checklist/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: [password]\n  oauth2_flows: []\n  first_party_oauth: false\n  openid_connect: false\nnote: >-\n  Rogers publishes no authentication documentation of its own and operates no first-party OAuth or\n  OpenID Connect surface — https://www.rogers.com/.well-known/openid-configuration,\n  https://api.rogers.com/.well-known/openid-configuration and\n  https://www.rogers.com/.well-known/oauth-authorization-server all return 404, and CIBA (the\n  authorization pattern CAMARA specifies for network-based authorization) appears nowhere on a Rogers\n  property. The only concrete auth model for a Rogers-branded API belongs to the Cisco IoT Control\n  Center platform that Rogers white-labels as Rogers Control Centre. That\
  \ model was confirmed live\n  against the Jasper REST tier during this round.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  interface: REST\n  credential: username + API key, colon-joined and Base64 encoded in the Authorization header\n  transport: HTTPS only (the REST APIs do not support plain HTTP)\n  realm: Jasper\n  evidence:\n  - kind: live-probe\n    request: GET https://restapi1.jasper.com/rws/api/v1/devices\n    status: 401\n    header: 'WWW-Authenticate: Basic realm=\"Jasper\"'\n    body: '{\"errorMessage\":\"Full authentication is required to access this resource\"}'\n    date: '2026-07-25'\n  - kind: docs\n    url: https://developer.cisco.com/docs/control-center/getting-started/\n    quote: >-\n      \"concatenate the user name and API key (separated by a colon) ... encrypt the resulting string\n      using Base64 ... set the authorization header value to 'Basic' followed by the encoded string.\"\n- name: licenseKey\n  type: apiKey\n  interface: SOAP\n  credential:\
  \ platform license key\n  note: >-\n    Cisco IoT Control Center SOAP API authentication. Rogers lists \"Access to applicable REST and SOAP\n    APIs\" as a Rogers Control Centre Advantage tier feature. The SOAP servlet mount is live on the\n    Rogers tenant host — every path under https://rogers.jasper.com/ws/service/ answers HTTP 405 to a\n    GET, consistent with a POST-only SOAP endpoint (a nonexistent service name answers 405 as well, so\n    individual service names could not be enumerated anonymously).\n- name: sharedSecret\n  type: signature\n  interface: PUSH (callbacks)\n  credential: shared secret used to sign and validate inbound callback requests\n  note: >-\n    Cisco IoT Control Center PUSH API callbacks. Cisco documents that \"for the PUSH API it is necessary\n    to configure a shared secret to validate the signature of incoming requests.\" Rogers publishes no\n    event catalog of its own.\nonboarding:\n  self_serve: false\n  note: >-\n    No self-serve signup exists\
  \ anywhere in the chain. API credentials are issued inside the Control\n    Centre console to customers with an existing Rogers Business contract; the console login for the\n    Rogers tenant is https://rogers.jasper.com/provision (HTTP 200, Cisco Control Center login).\n    Cisco separately offers a time-reserved DevNet sandbox for the platform\n    (https://rws-jpotest.jasper.com/rws/api/) with credentials mailed on reservation — that is a Cisco\n    DevNet facility, not a Rogers sandbox.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rogers/refs/heads/main/authentication/rogers-authentication.yml
summary_line: http · 3 schemes
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- 5G
- Network APIs
- CAMARA
- Identity Verification
- SIM Swap
- IoT
- Media
---
