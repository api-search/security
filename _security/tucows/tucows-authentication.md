---
api_key_in:
- header
auth_types:
- apiKey
- signature
description: 'OpenSRS uses an HTTPS POST protocol with request signing rather than OAuth. Each request carries two HTTP headers: `X-Username` (the reseller username) and `X-Signature` (a signature computed over the XML request body and the reseller API key). There are no OAuth flows and no bearer tokens; the API key is a long-lived secret issued in the Reseller Control Panel.'
kind: authentication
layout: security
method: searched
name: Tucows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tucows secures its APIs with apiKey and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tucows
provider_slug: tucows
scheme_count: 2
schemes:
- description: Reseller username identifying the calling account.
  in: header
  name: X-Username
  parameter: X-Username
  type: apiKey
- algorithm: md5
  computation: 'signature = md5( md5( xml_body + api_key ) + api_key ) (double MD5: first md5 of the XML body concatenated with the API key, then md5 of that hex digest concatenated with the API key again).'
  description: Per-request signature binding the XML body to the reseller API key.
  in: header
  name: X-Signature
  parameter: X-Signature
  type: signature
slug: tucows-authentication
source_filename: tucows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://domains.opensrs.guide/docs/quickstart\ndocs: https://domains.opensrs.guide/docs/quickstart\napi: OpenSRS Domains and TLS/SSL API\nsummary:\n  types: [apiKey, signature]\n  api_key_in: [header]\n  scheme: reseller-username-plus-md5-signature\n  oauth2_flows: []\ndescription: >-\n  OpenSRS uses an HTTPS POST protocol with request signing rather than OAuth.\n  Each request carries two HTTP headers: `X-Username` (the reseller username)\n  and `X-Signature` (a signature computed over the XML request body and the\n  reseller API key). There are no OAuth flows and no bearer tokens; the API key\n  is a long-lived secret issued in the Reseller Control Panel.\ncredentials:\n  reseller_username: The reseller account username.\n  api_key:\n    where: Reseller Control Panel > Account Settings > (gear icon) > API settings tab\n    console: https://manage.opensrs.com\n    note: Long-lived secret; also gate access by whitelisting your\
  \ server IP in the control panel.\nschemes:\n  - name: X-Username\n    type: apiKey\n    in: header\n    parameter: X-Username\n    description: Reseller username identifying the calling account.\n  - name: X-Signature\n    type: signature\n    in: header\n    parameter: X-Signature\n    algorithm: md5\n    computation: >-\n      signature = md5( md5( xml_body + api_key ) + api_key )\n      (double MD5: first md5 of the XML body concatenated with the API key,\n      then md5 of that hex digest concatenated with the API key again).\n    description: Per-request signature binding the XML body to the reseller API key.\nip_allowlisting:\n  supported: true\n  note: >-\n    API access must be enabled and the calling server IP address whitelisted in\n    the Reseller Control Panel; requests from non-whitelisted IPs return\n    \"Access denied: invalid IP address\" (response code 400).\ntransport:\n  protocol: HTTPS POST\n  body: XML (OPS envelope)\n  content_type: text/xml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tucows/refs/heads/main/authentication/tucows-authentication.yml
summary_line: apiKey/signature · 2 schemes
tags:
- Company
- Infrastructure
- Domains
- DNS
- SSL
- Email
- Registrar
- Telecom
---
