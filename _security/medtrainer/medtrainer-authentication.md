---
api_key_in:
- header
api_specs:
- filename: medtrainer-public-api-openapi.json
  format: json
  label: MedTrainer Public API
  slug: medtrainer-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-public-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Medtrainer Authentication
name_suffix: Authentication
oauth_flows: []
overview: MedTrainer secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MedTrainer
provider_slug: medtrainer
scheme_count: 2
schemes:
- description: Preferred authentication header for protected endpoints.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/medtrainer-public-api-openapi.json
  type: apiKey
- bearerFormat: API key
  description: 'Alternative authentication scheme using `Authorization: Bearer <token>`. The bearer value is the same API key, not a separately issued OAuth access token.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/medtrainer-public-api-openapi.json
  type: http
slug: medtrainer-authentication
source_filename: medtrainer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  openapi/medtrainer-public-api-openapi.json;\n  https://api.medtrainer.com/docs#section/Getting-started;\n  https://auth.medtrainer.com/.well-known/openid-configuration\ndocs: https://api.medtrainer.com/docs#section/Getting-started\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  primary: X-API-Key header\n  oauth2: false\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Preferred authentication header for protected endpoints.\n  sources:\n  - openapi/medtrainer-public-api-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Alternative authentication scheme using `Authorization: Bearer <token>`. The bearer value is the same API key, not a separately issued OAuth access token.'\n  sources:\n  - openapi/medtrainer-public-api-openapi.json\nkey_issuance:\n  self_service: true\n  requires_existing_account:\
  \ true\n  flow:\n  - Sign in to the MedTrainer platform with an account holding Super Admin or Admin permissions.\n  - Open Organization from the left-hand menu.\n  - Expand \"Organization Management\" and open \"API keys manager\".\n  - Create an API key group, supplying a name and description.\n  - The group is created with a \"Default\" key in Inactive status; change the status to Active before use.\n  source: 'https://api.medtrainer.com/docs#section/Step-by-step (also carried verbatim in info.description of the OpenAPI)'\n  note: >-\n    Keys cannot be obtained without a paying MedTrainer tenant and an admin role. There is no\n    developer sandbox, no free tier and no anonymous key issuance, so the API is customer-gated\n    even though the reference documentation is fully public.\nunauthenticated_behavior:\n  status: 401\n  media_type: application/fhir+json\n  body: '{\"resourceType\":\"OperationOutcome\",\"issue\":[{\"severity\":\"error\",\"code\":\"login\",\"details\":{\"text\"\
  :\"Missing or invalid authentication credentials. Provide an API key using the X-API-Key header or Authorization: Bearer <token>.\"}}]}'\n  observed: 'Probed 2026-08-25 against https://api.medtrainer.com/api/v1/locations — the host returns this for every path, including /.well-known/*.'\nrelated_surfaces:\n- surface: MedTrainer platform sign-in\n  protocol: OpenID Connect / OAuth 2.0\n  issuer: https://auth.medtrainer.com/\n  discovery: well-known/medtrainer-auth-openid-configuration.json\n  note: 'Auth0 on a MedTrainer custom domain. Supports authorization_code with PKCE (S256), refresh tokens, device code, private_key_jwt, and MFA challenge. Governs the LMS/web app, not the Public API.'\n- surface: MedTrainer MCP server\n  protocol: OAuth 2.0 (RFC 8414 + RFC 9728)\n  issuer: https://medtrainer.com\n  scope: mcp\n  note: See mcp/medtrainer-mcp.yml.\ngaps:\n- 'No token rotation, expiry or revocation policy is published for API keys.'\n- 'No key prefix convention is documented, so a leaked\
  \ key is not self-identifying.'\n- 'No mTLS, no signed requests, and no IP allow-listing are documented for a directory API that carries practitioner PII (names, home addresses, phone, email, NPI, birth place).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/authentication/medtrainer-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Healthcare
- Compliance
- Credentialing
- Learning Management
- Provider Directory
- FHIR
- HL7
- Training
- Risk Management
- SaaS
---
