---
api_key_in:
- header
- query
auth_types:
- apiKey
- custom-session-token
- mutualTLS
- none
description: ''
kind: authentication
layout: security
method: searched
name: Pjm Authentication
name_suffix: Authentication
oauth_flows: []
overview: PJM Interconnection secures its APIs with apiKey, custom-session-token, mutualTLS, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PJM Interconnection
provider_slug: pjm
scheme_count: 5
schemes:
- applies_to:
  - PJM Data Miner 2 API (https://api.pjm.com/api/v1)
  - PJM Data Miner 2 training API (https://api-train.pjm.com/api/v1)
  constraint: One subscription key is bound to one unique email address; unlike other PJM tools, no other user accounts may be tied to that email address (Data Miner FAQ). System accounts are allowed provided a valid email address is attached to the user id and the company CAM provisions it for traceability.
  cost: free
  in: header
  name: DataMinerSubscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  platform: Azure API Management
  provisioning: Requires a PJM Tools username provisioned for Data Miner. Member companies request access via PJM Account Manager > Account Access > Request Access > Data Miner API. Non-member companies email accountmanager@pjm.com with the statement "I confirm that the PJM Data will be used for internal business purposes only", their Account Manager user id and their subscribing email address. A Customer Account Manager approves; the key is then read from View Profile > Your Subscriptions.
  source: https://www.pjm.com/-/media/DotCom/etools/data-miner-2/data-miner-2-api-guide.ashx
  type: apiKey
  verified: GET https://api.pjm.com/api/v1/gen_by_fuel returned HTTP 401 anonymously on 2026-07-27
- applies_to:
  - PJM Data Miner 2 API (https://api.pjm.com/api/v1)
  in: query
  name: DataMinerSubscriptionKeyQuery
  note: Same credential as the header form; the guide documents appending &subscription-key=<yourkey> to a request URL for browser/Excel/data-connection use.
  parameter: subscription-key
  source: https://www.pjm.com/-/media/DotCom/etools/data-miner-2/data-miner-2-api-guide.ashx
  type: apiKey
- applies_to:
  - PJM OASIS Template API
  - PJM InSchedule Browserless API
  - PJM eDART Browserless API
  - other PJM eTools browserless interfaces
  flow: POST https://sso.pjm.com/access/authenticate/ with the headers X-OpenAM-Username and X-OpenAM-Password. The JSON response carries a tokenId, which is presented as the pjmauth cookie on subsequent tool API calls and released with POST https://sso.pjm.com/access/logout/.
  in: cookie
  name: PJMSingleSignOnToken
  parameter: pjmauth
  platform: ForgeRock OpenAM
  revocation_endpoint: https://sso.pjm.com/access/logout/
  source: https://www.pjm.com/-/media/DotCom/etools/pjm-browserless-authentication-guide.pdf
  token_endpoint: https://sso.pjm.com/access/authenticate/
  training_parameter: pjmauthtrain
  type: custom-session-token
  verified: GET https://sso.pjm.com/access/authenticate/ returned HTTP 405 Method Not Allowed on 2026-07-27, confirming the documented POST-only endpoint
- applies_to:
  - Custom-code REST clients against PJM eTools
  flow: Two-way TLS with a PJM-issued client certificate against the access/authenticate/pjmauthcert endpoint, presented alongside credentials to obtain the SSO token.
  name: PJMClientCertificate
  source: https://www.pjm.com/-/media/DotCom/etools/security/pki-authentication-guide.pdf
  type: mutualTLS
- applies_to:
  - PJM Messages Public Web Service (https://messages.pjm.com/messages/rest/public)
  - PJM OASIS public information page (https://pjmoasis.pjm.com/OASIS/PJM/INFO.HTM)
  name: PublicAnonymous
  note: The Messages public web service and the NAESB WEQ-002-4.5.2 mandated OASIS Online Resources posting are served with no credential of any kind.
  type: none
  verified: GET https://messages.pjm.com/messages/rest/public/messages returned HTTP 200 anonymously on 2026-07-27
slug: pjm-authentication
source_filename: pjm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  PJM Data Miner API Guide (v15, 02/10/2026), PJM Browserless Authentication Guide,\n  PJM PKI-Based Authentication Guide, PJM OASIS API User Guide (Rev 04, 2023-01-27),\n  plus anonymous probes of api.pjm.com, sso.pjm.com, apiportal.pjm.com and\n  messages.pjm.com on 2026-07-27.\ndocs: https://www.pjm.com/markets-and-operations/etools/security.aspx\nsummary:\n  types: [apiKey, custom-session-token, mutualTLS, none]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  openid_connect: false\n  note: >-\n    PJM publishes no OAuth 2.0 or OpenID Connect surface. GET\n    https://sso.pjm.com/.well-known/openid-configuration returned HTTP 404 and\n    https://www.pjm.com/.well-known/openid-configuration returned the pjm.com HTML\n    shell (soft 404). Authentication is split three ways: an Azure API Management\n    subscription key for Data Miner 2, a ForgeRock OpenAM session token (with an\n    optional/required PKI client\
  \ certificate) for the eTools surfaces, and fully\n    anonymous access for the public Messages web service.\nschemes:\n- name: DataMinerSubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  applies_to:\n  - PJM Data Miner 2 API (https://api.pjm.com/api/v1)\n  - PJM Data Miner 2 training API (https://api-train.pjm.com/api/v1)\n  platform: Azure API Management\n  cost: free\n  provisioning: >-\n    Requires a PJM Tools username provisioned for Data Miner. Member companies\n    request access via PJM Account Manager > Account Access > Request Access > Data\n    Miner API. Non-member companies email accountmanager@pjm.com with the statement\n    \"I confirm that the PJM Data will be used for internal business purposes only\",\n    their Account Manager user id and their subscribing email address. A Customer\n    Account Manager approves; the key is then read from View Profile > Your\n    Subscriptions.\n  constraint: >-\n    One subscription key is bound\
  \ to one unique email address; unlike other PJM\n    tools, no other user accounts may be tied to that email address (Data Miner FAQ).\n    System accounts are allowed provided a valid email address is attached to the\n    user id and the company CAM provisions it for traceability.\n  source: https://www.pjm.com/-/media/DotCom/etools/data-miner-2/data-miner-2-api-guide.ashx\n  verified: 'GET https://api.pjm.com/api/v1/gen_by_fuel returned HTTP 401 anonymously on 2026-07-27'\n- name: DataMinerSubscriptionKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  applies_to:\n  - PJM Data Miner 2 API (https://api.pjm.com/api/v1)\n  note: >-\n    Same credential as the header form; the guide documents appending\n    &subscription-key=<yourkey> to a request URL for browser/Excel/data-connection\n    use.\n  source: https://www.pjm.com/-/media/DotCom/etools/data-miner-2/data-miner-2-api-guide.ashx\n- name: PJMSingleSignOnToken\n  type: custom-session-token\n  in: cookie\n  parameter:\
  \ pjmauth\n  training_parameter: pjmauthtrain\n  applies_to:\n  - PJM OASIS Template API\n  - PJM InSchedule Browserless API\n  - PJM eDART Browserless API\n  - other PJM eTools browserless interfaces\n  platform: ForgeRock OpenAM\n  flow: >-\n    POST https://sso.pjm.com/access/authenticate/ with the headers X-OpenAM-Username\n    and X-OpenAM-Password. The JSON response carries a tokenId, which is presented as\n    the pjmauth cookie on subsequent tool API calls and released with POST\n    https://sso.pjm.com/access/logout/.\n  token_endpoint: https://sso.pjm.com/access/authenticate/\n  revocation_endpoint: https://sso.pjm.com/access/logout/\n  source: https://www.pjm.com/-/media/DotCom/etools/pjm-browserless-authentication-guide.pdf\n  verified: 'GET https://sso.pjm.com/access/authenticate/ returned HTTP 405 Method Not Allowed on 2026-07-27, confirming the documented POST-only endpoint'\n- name: PJMClientCertificate\n  type: mutualTLS\n  applies_to:\n  - Custom-code REST clients against\
  \ PJM eTools\n  flow: >-\n    Two-way TLS with a PJM-issued client certificate against the\n    access/authenticate/pjmauthcert endpoint, presented alongside credentials to\n    obtain the SSO token.\n  source: https://www.pjm.com/-/media/DotCom/etools/security/pki-authentication-guide.pdf\n- name: PublicAnonymous\n  type: none\n  applies_to:\n  - PJM Messages Public Web Service (https://messages.pjm.com/messages/rest/public)\n  - PJM OASIS public information page (https://pjmoasis.pjm.com/OASIS/PJM/INFO.HTM)\n  note: >-\n    The Messages public web service and the NAESB WEQ-002-4.5.2 mandated OASIS\n    Online Resources posting are served with no credential of any kind.\n  verified: 'GET https://messages.pjm.com/messages/rest/public/messages returned HTTP 200 anonymously on 2026-07-27'\ntransport:\n  tls_minimum: TLS 1.2\n  note: >-\n    \"In general, Tls1.2 is required for all PJM tools, including Data Miner.\" PJM\n    retired TLS 1.0/1.1 from internet-facing applications in the April\
  \ 2022 Data\n    Miner release, and its security appliance began enforcing strict HTTP protocol\n    rules on 2025-11-01 (an HTTP GET carrying a body is rejected).\n  source: https://www.pjm.com/-/media/DotCom/etools/data-miner-2/data-miner-2-api-guide.ashx\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pjm/refs/heads/main/authentication/pjm-authentication.yml
summary_line: apiKey/custom-session-token/mutualTLS/none · 5 schemes
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Grid
- System Operator
- Wholesale Electricity
- Transmission
- Market Data
- Demand Response
---
