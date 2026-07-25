---
api_key_in:
- query
auth_types:
- apiKey
- token
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Euronext Authentication
name_suffix: Authentication
oauth_flows: []
overview: Euronext secures its APIs with apiKey, token, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Euronext
provider_slug: euronext
scheme_count: 4
schemes:
- api: Euronext Web Services (Market Data / Historical / Indices)
  description: 'The Euronext Web Services JSON API authenticates with an authentication key

    passed as the authKey query parameter on the gateway.euronext.com/api

    endpoints (e.g. /api/instrumentDetail, /api/intraday). The URL and Key are

    provided by Euronext to the client at integration onboarding; requests use

    the POST HTTP method only (GET is not supported for the EOD Summary service).

    An unauthenticated request to https://gateway.euronext.com/api/instrumentDetail

    returns HTTP 401 (probed 2026-07-22).

    '
  in: query
  name: EWS authKey
  parameter: authKey
  sources:
  - https://connect2.euronext.com/sites/default/files/documentation/data/EWS%20API%20-%20Indices%20-%20Client%20Specification_v1.3_27.01.2020.pdf
  - https://connect2.euronext.com/sites/default/files/documentation/data/ews_api_-_historical_data_client_specification.pdf
  type: apiKey
- api: Euronext Saturn Reporting API
  description: 'The client first calls the AuthenticateUser logon function

    (/SaturnWebServices/rest/Authentication/AuthenticateUser) over HTTPS with the

    Saturn username and password - the Username:Password concatenation is MD5

    encrypted then base64 encoded (hexadecimal, lowercase) and carried in the

    Authorization HTTP header. Saturn validates the credentials and returns a

    session token that must be sent in the Authorization header of every

    subsequent request. Tokens expire after a configurable period ("Token

    expired" error); Saturn pins the client IP from the logon request and

    rejects requests from other IPs; only one active session per credential is

    allowed (a new logon invalidates the previous session). Logon status codes:

    200 Success, 401 Access denied, 504 Session expired.

    '
  in: header
  name: Saturn session token
  parameter: Authorization
  sources:
  - https://www.euronext.com/sites/www.euronext.com/files/euronext-saturn-web_services_specifications_2.8.8.pdf
  type: token
- api: Euronext Saturn Reporting API
  description: 'In addition to token authentication, Saturn uses certificate-based mutual

    authentication - the client presents a client certificate (a DigiCert-issued

    .pfx is distributed by Euronext, with a published DigiCert certificate

    utility for conversion) and both parties verify each other''s certificates

    before the encrypted channel is established.

    '
  name: Saturn mutual TLS
  sources:
  - https://www.euronext.com/sites/www.euronext.com/files/euronext-saturn-web_services_specifications_2.8.8.pdf
  type: mutualTLS
- api: Euronext Optiq Market Data Gateway
  description: 'Not an HTTP API - the Optiq Market Data Gateway is a UDP multicast SBE feed.

    Access control is contractual and network-level: a market data agreement,

    entitlement management, and connectivity provisioning (no HTTP

    authentication scheme).

    '
  name: Optiq MDG entitlement
  sources:
  - https://www.euronext.com/en/data/how-access-market-data/euronext-optiq-mdg-cloud
  type: none
slug: euronext-authentication
source_filename: euronext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: |\n  Euronext public client-specification PDFs (fetched and read 2026-07-22):\n  - https://www.euronext.com/sites/www.euronext.com/files/euronext-saturn-web_services_specifications_2.8.8.pdf\n  - https://connect2.euronext.com/sites/default/files/documentation/data/EWS%20API%20-%20Indices%20-%20Client%20Specification_v1.3_27.01.2020.pdf\n  - https://connect2.euronext.com/sites/default/files/documentation/data/ews_api_-_historical_data_client_specification.pdf\nsummary:\n  types: [apiKey, token, mutualTLS]\n  api_key_in: [query]\n  oauth2_flows: []\n  note: No OAuth2/OIDC anywhere. All credentials are issued by Euronext at\n    onboarding; there is no self-serve signup.\nschemes:\n- name: EWS authKey\n  api: Euronext Web Services (Market Data / Historical / Indices)\n  type: apiKey\n  in: query\n  parameter: authKey\n  description: |\n    The Euronext Web Services JSON API authenticates with an authentication key\n    passed\
  \ as the authKey query parameter on the gateway.euronext.com/api\n    endpoints (e.g. /api/instrumentDetail, /api/intraday). The URL and Key are\n    provided by Euronext to the client at integration onboarding; requests use\n    the POST HTTP method only (GET is not supported for the EOD Summary service).\n    An unauthenticated request to https://gateway.euronext.com/api/instrumentDetail\n    returns HTTP 401 (probed 2026-07-22).\n  sources:\n  - https://connect2.euronext.com/sites/default/files/documentation/data/EWS%20API%20-%20Indices%20-%20Client%20Specification_v1.3_27.01.2020.pdf\n  - https://connect2.euronext.com/sites/default/files/documentation/data/ews_api_-_historical_data_client_specification.pdf\n- name: Saturn session token\n  api: Euronext Saturn Reporting API\n  type: token\n  in: header\n  parameter: Authorization\n  description: |\n    The client first calls the AuthenticateUser logon function\n    (/SaturnWebServices/rest/Authentication/AuthenticateUser) over HTTPS\
  \ with the\n    Saturn username and password - the Username:Password concatenation is MD5\n    encrypted then base64 encoded (hexadecimal, lowercase) and carried in the\n    Authorization HTTP header. Saturn validates the credentials and returns a\n    session token that must be sent in the Authorization header of every\n    subsequent request. Tokens expire after a configurable period (\"Token\n    expired\" error); Saturn pins the client IP from the logon request and\n    rejects requests from other IPs; only one active session per credential is\n    allowed (a new logon invalidates the previous session). Logon status codes:\n    200 Success, 401 Access denied, 504 Session expired.\n  sources:\n  - https://www.euronext.com/sites/www.euronext.com/files/euronext-saturn-web_services_specifications_2.8.8.pdf\n- name: Saturn mutual TLS\n  api: Euronext Saturn Reporting API\n  type: mutualTLS\n  description: |\n    In addition to token authentication, Saturn uses certificate-based mutual\n\
  \    authentication - the client presents a client certificate (a DigiCert-issued\n    .pfx is distributed by Euronext, with a published DigiCert certificate\n    utility for conversion) and both parties verify each other's certificates\n    before the encrypted channel is established.\n  sources:\n  - https://www.euronext.com/sites/www.euronext.com/files/euronext-saturn-web_services_specifications_2.8.8.pdf\n- name: Optiq MDG entitlement\n  api: Euronext Optiq Market Data Gateway\n  type: none\n  description: |\n    Not an HTTP API - the Optiq Market Data Gateway is a UDP multicast SBE feed.\n    Access control is contractual and network-level: a market data agreement,\n    entitlement management, and connectivity provisioning (no HTTP\n    authentication scheme).\n  sources:\n  - https://www.euronext.com/en/data/how-access-market-data/euronext-optiq-mdg-cloud\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euronext/refs/heads/main/authentication/euronext-authentication.yml
summary_line: apiKey/token/mutualTLS · 4 schemes
tags:
- Financial
- Market Data
- Stocks
- Exchange
- Real-Time
- Historical Data
- Indices
- Reference Data
- Derivatives
- Regulatory Reporting
---
