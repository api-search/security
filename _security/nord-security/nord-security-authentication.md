---
api_key_in:
- header
api_specs:
- filename: nord-security-nordstellar-enterprise-data-api-openapi.json
  format: json
  label: NordStellar Enterprise Data API
  slug: nordstellar-enterprise-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-enterprise-data-api-openapi.json
- filename: nord-security-nordstellar-company-risk-scoring-api-openapi.json
  format: json
  label: NordStellar Company Risk Scoring API
  slug: nordstellar-company-risk-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json
- filename: nord-security-nordstellar-cybersec-api-openapi.json
  format: json
  label: NordStellar Cybersec API
  slug: nordstellar-cybersec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-cybersec-api-openapi.json
- filename: nord-security-nordstellar-partners-api-openapi.json
  format: json
  label: NordStellar Partners API
  slug: nordstellar-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-partners-api-openapi.json
- filename: nord-security-nordstellar-platform-integration-api-v3-openapi.json
  format: json
  label: NordStellar Platform Integrations API
  slug: nordstellar-platform-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-platform-integration-api-v3-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nord Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nord Security secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nord Security
provider_slug: nord-security
scheme_count: 6
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json
  type: apiKey
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json
  - openapi/nord-security-nordstellar-enterprise-data-api-openapi.json
  type: http
- bearerFormat: JWT
  description: 'Set token with a prefix like this: `token:69405a802dba4f57804e5fff11061946a579d159d1a51760d19a50aec241adc9`'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/nord-security-nordstellar-cybersec-api-openapi.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/nord-security-nordstellar-enterprise-data-api-openapi.json
  type: apiKey
- description: API key to access the API
  in: header
  name: ApiKey
  parameter: Api-Key
  sources:
  - openapi/nord-security-nordstellar-partners-api-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: Please enter a valid token.
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/nord-security-nordstellar-platform-integration-api-v1-openapi.json
  - openapi/nord-security-nordstellar-platform-integration-api-v2-openapi.json
  - openapi/nord-security-nordstellar-platform-integration-api-v3-openapi.json
  type: http
slug: nord-security-authentication
source_filename: nord-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\ndocs: https://docs.nordstellar.com/enterprise-apis/product-integrations/authentication\ndocs_notes:\n- 'Two documented methods for the enterprise APIs: API key header and HTTP Basic.'\n- API tokens are created, listed and revoked in the NordStellar platform UI; docs cover rotation, access controls and audit/monitoring practice.\n- Published guidance explicitly warns against exposing API keys in client-side code.\nnon_spec_schemes:\n- surface: NordLayer Partner / MSP API\n  scheme: apiKey\n  detail: >-\n    Keys are self-issued in the NordLayer Service Management Portal (Integrations > Custom), with a\n    named key, an explicit expiry and one-time visibility, supporting rotation without downtime.\n  docs: https://help.nordlayer.com/docs/api-key-management-for-smp\n- surface: NordLayer SCIM 2.0 provisioning\n  scheme: http bearer (SCIM secret token)\n  detail: >-\n    A Secret Token is issued in the NordLayer Control Panel under Settings\
  \ > Access management and\n    pasted into the Okta or Microsoft Entra ID provisioning configuration.\n  docs: https://help.nordlayer.com/docs/user-provisioning\n- surface: NordStellar MCP server\n  scheme: bearer session established by browser login\n  detail: >-\n    The local nordstellar-mcp proxy opens a browser window for NordStellar login and stores the session\n    in the OS credential store under the service name \"NordStellar MCP\", refreshing tokens as needed.\n    An unauthenticated tools/list returns HTTP 401 \"no bearer token\". No RFC 8414 or RFC 9728 discovery\n    document is published.\n  docs: https://docs.nordstellar.com/platform/mcp/setup\n- surface: NordLayer / NordPass administrator sign-in\n  scheme: SSO + SCIM\n  detail: >-\n    SSO via Google Workspace, Okta, Microsoft Entra ID, JumpCloud and OneLogin, with centrally enforced\n    2FA (SMS or TOTP) and the option to disable username/password login entirely.\n  docs: https://help.nordlayer.com/docs/single-sign-on-sso-setup\n\
  oauth2:\n  present: false\n  note: >-\n    No oauth2 or openIdConnect security scheme appears in any of the seven harvested specs, and\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404 on every\n    host probed. scopes/ is therefore not emitted — there is no scope surface to record.\nderived_from: openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json, openapi/nord-security-nordstellar-cybersec-api-openapi.json,\n  openapi/nord-security-nordstellar-enterprise-data-api-openapi.json, openapi/nord-security-nordstellar-partners-api-openapi.json,\n  openapi/nord-security-nordstellar-platform-integration-api-v1-openapi.json, openapi/nord-security-nordstellar-platform-integration-api-v2-openapi.json,\n  openapi/nord-security-nordstellar-platform-integration-api-v3-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n \
  \ sources:\n  - openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json\n  - openapi/nord-security-nordstellar-enterprise-data-api-openapi.json\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Set token with a prefix like this: `token:69405a802dba4f57804e5fff11061946a579d159d1a51760d19a50aec241adc9`'\n  sources:\n  - openapi/nord-security-nordstellar-cybersec-api-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/nord-security-nordstellar-enterprise-data-api-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: API key to access the API\n  sources:\n  - openapi/nord-security-nordstellar-partners-api-openapi.json\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description:\
  \ Please enter a valid token.\n  sources:\n  - openapi/nord-security-nordstellar-platform-integration-api-v1-openapi.json\n  - openapi/nord-security-nordstellar-platform-integration-api-v2-openapi.json\n  - openapi/nord-security-nordstellar-platform-integration-api-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/authentication/nord-security-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Cybersecurity
- Threat Intelligence
- Dark Web Monitoring
- Attack Surface Management
- Breach Intelligence
- VPN
- Password Management
- Network Security
- Zero Trust
- Privacy
- MCP
- Agent Skills
- gRPC
- Company
---
