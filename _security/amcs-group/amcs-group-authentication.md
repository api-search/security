---
api_key_in:
- query
- cookie
api_specs:
- filename: amcs-group-erp-openapi-original.json
  format: json
  label: AMCS Platform ERP REST API
  slug: amcs-platform-erp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-erp-openapi-original.json
- filename: amcs-group-core-openapi-original.json
  format: json
  label: AMCS Core API
  slug: amcs-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-core-openapi-original.json
- filename: amcs-group-pay-openapi-original.json
  format: json
  label: AMCS Pay External API
  slug: amcs-pay-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-pay-openapi-original.json
- filename: amcs-group-scale-openapi-original.json
  format: json
  label: AMCS Scale REST API
  slug: amcs-scale-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-scale-openapi-original.json
- filename: amcs-group-tlv-openapi-original.json
  format: json
  label: AMCS TLV External API
  slug: amcs-tlv-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-tlv-openapi-original.json
- filename: amcs-group-visionai-openapi-original.json
  format: json
  label: AMCS Vision AI External API
  slug: amcs-vision-ai-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/openapi/amcs-group-visionai-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Amcs Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMCS Group secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AMCS Group
provider_slug: amcs-group
scheme_count: 3
schemes:
- description: Personal Access Token (PAT) presented as the PrivateKey query parameter to POST /erp/api/authTokens to start a session. Sandbox PATs are issued via the developer stack forum.
  in: query
  name: privateKey
  parameter: PrivateKey
  sources:
  - quickstart/READ ME.md (amcsplatform/amcsrestapi)
  type: apiKey
- description: Session token returned by the authTokens endpoint in Set-Cookie, replayed as a Cookie header on every data request.
  in: cookie
  name: sessionCookie
  parameter: session
  sources:
  - quickstart/READ ME.md (amcsplatform/amcsrestapi)
  type: apiKey
- description: AMCS Pay external API session cookie.
  in: cookie
  name: cookieAuth
  parameter: Platform.PAY.SessionToken
  sources:
  - openapi/amcs-group-pay-openapi-original.json
  type: apiKey
slug: amcs-group-authentication
source_filename: amcs-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/amcs-group-pay-openapi-original.json\ndocs: https://github.com/amcsplatform/amcsrestapi/tree/master/quickstart\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - cookie\n  model: >-\n    The AMCS Platform REST API uses a two-step Personal Access Token (PAT) plus\n    session-cookie model. A client first POSTs its PAT (PrivateKey) to the\n    authTokens endpoint; on success the response returns authResult \"ok\" and a\n    session token in a Set-Cookie header. That session cookie is then sent on\n    every subsequent data request. AMCS Pay uses the same shape with a\n    Platform.PAY.SessionToken cookie.\nschemes:\n- name: privateKey\n  type: apiKey\n  in: query\n  parameter: PrivateKey\n  description: >-\n    Personal Access Token (PAT) presented as the PrivateKey query parameter to\n    POST /erp/api/authTokens to start a session. Sandbox PATs are issued via the\n    developer stack forum.\n  sources:\n\
  \  - quickstart/READ ME.md (amcsplatform/amcsrestapi)\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: >-\n    Session token returned by the authTokens endpoint in Set-Cookie, replayed as\n    a Cookie header on every data request.\n  sources:\n  - quickstart/READ ME.md (amcsplatform/amcsrestapi)\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: Platform.PAY.SessionToken\n  description: AMCS Pay external API session cookie.\n  sources:\n  - openapi/amcs-group-pay-openapi-original.json\nendpoints:\n  auth_token: POST /erp/api/authTokens?PrivateKey={PAT}\n  auth_result_field: authResult\nnotes:\n- No OAuth2 / OpenID Connect surface is declared in any published spec; scopes/ is not applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amcs-group/refs/heads/main/authentication/amcs-group-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Waste Management
- Recycling
- Transport
- Logistics
- Environmental
- ERP
- Payments
- Artificial Intelligence
- SaaS
---
