---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Forcepoint Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Forcepoint secures its APIs with oauth2, apiKey, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Forcepoint
provider_slug: forcepoint
scheme_count: 4
schemes:
- detail: 'OAuth 2.0. Configure API permission levels under Settings > API Interface > OAuth, generate a token, then send Authorization: Bearer <token>. Adding a new scope requires minting a new token. Config/Log/IP APIs plus SCIM user & group provisioning are gated by scope.'
  docs: https://help.forcepoint.com/fpone/deploy/rhtml/guid-18f77855-8dc9-436a-9fba-179f06a81066.html
  name: sse_oauth2
  product: Forcepoint Data Security Cloud | SSE (Forcepoint ONE)
  scheme: bearer
  type: oauth2
- detail: API key issued by creating an API Client element in the SMC with the required privileges; the key authenticates session.login() in the fp-NGFW-SMC-python SDK.
  docs: https://support.forcepoint.com/s/article/How-to-Start-Using-SMC-API
  in: header
  name: ngfw_smc_api_key
  product: Forcepoint NGFW Security Management Center (SMC) API
  type: apiKey
- detail: Username/password (management-server admin credentials) exchanged for a session/bearer token used on subsequent policy-management calls.
  docs: https://help.forcepoint.com/dlp/90/restapi/index.html
  name: dlp_basic
  product: Forcepoint DLP REST API
  scheme: basic
  type: http
- detail: HTTP basic authentication against the appliance host.
  docs: https://help.forcepoint.com/docs/appliance/v85/appliance_api/how_to_use.html
  name: appliance_basic
  product: Forcepoint Appliance REST API
  scheme: basic
  type: http
slug: forcepoint-authentication
source_filename: forcepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.forcepoint.com/fpone/deploy/rhtml/guid-18f77855-8dc9-436a-9fba-179f06a81066.html\ndocs: https://help.forcepoint.com/fpone/deploy/rhtml/guid-d35197e0-5924-4838-af15-6298cf9e7b50.html\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  note: >-\n    Forcepoint ships several product REST APIs with different auth models; there is no single\n    unified gateway. Auth is documented per product in help.forcepoint.com.\nschemes:\n  - name: sse_oauth2\n    product: Forcepoint Data Security Cloud | SSE (Forcepoint ONE)\n    type: oauth2\n    scheme: bearer\n    detail: >-\n      OAuth 2.0. Configure API permission levels under Settings > API Interface > OAuth,\n      generate a token, then send Authorization: Bearer <token>. Adding a new scope requires\n      minting a new token. Config/Log/IP APIs plus SCIM user & group provisioning are gated by scope.\n    docs: https://help.forcepoint.com/fpone/deploy/rhtml/guid-18f77855-8dc9-436a-9fba-179f06a81066.html\n\
  \  - name: ngfw_smc_api_key\n    product: Forcepoint NGFW Security Management Center (SMC) API\n    type: apiKey\n    in: header\n    detail: >-\n      API key issued by creating an API Client element in the SMC with the required privileges;\n      the key authenticates session.login() in the fp-NGFW-SMC-python SDK.\n    docs: https://support.forcepoint.com/s/article/How-to-Start-Using-SMC-API\n  - name: dlp_basic\n    product: Forcepoint DLP REST API\n    type: http\n    scheme: basic\n    detail: >-\n      Username/password (management-server admin credentials) exchanged for a session/bearer token\n      used on subsequent policy-management calls.\n    docs: https://help.forcepoint.com/dlp/90/restapi/index.html\n  - name: appliance_basic\n    product: Forcepoint Appliance REST API\n    type: http\n    scheme: basic\n    detail: HTTP basic authentication against the appliance host.\n    docs: https://help.forcepoint.com/docs/appliance/v85/appliance_api/how_to_use.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forcepoint/refs/heads/main/authentication/forcepoint-authentication.yml
summary_line: oauth2/apiKey/http · 4 schemes
tags:
- Company
- Cybersecurity
- Security
- Data Loss Prevention
- SASE
- Security Service Edge
- Firewall
- Data Security
- Cloud Security
---
