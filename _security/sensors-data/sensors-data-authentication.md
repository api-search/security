---
api_key_in: []
api_specs:
- filename: sensors-data-analytics-channel-v1-openapi.yml
  format: yaml
  label: Sensors Analytics OpenAPI (神策分析)
  slug: sensors-analytics-openapi-神策分析
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-analytics-channel-v1-openapi.yml
- filename: sensors-data-horizon-catalog-v1-openapi.yml
  format: yaml
  label: Sensors Horizon CDP OpenAPI (神策数界)
  slug: sensors-horizon-cdp-openapi-神策数界
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-horizon-catalog-v1-openapi.yml
- filename: sensors-data-focus-express-action-channel-v1-openapi.yml
  format: yaml
  label: Sensors Focus OpenAPI (神策智能运营)
  slug: sensors-focus-openapi-神策智能运营
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-focus-express-action-channel-v1-openapi.yml
- filename: sensors-data-portal-identity-v2-openapi.yml
  format: yaml
  label: Sensors Portal OpenAPI (神策业务门户)
  slug: sensors-portal-openapi-神策业务门户
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/openapi/sensors-data-portal-identity-v2-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sensors Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensors Data declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Sensors Data
provider_slug: sensors-data
scheme_count: 4
schemes:
- coverage: 252 of 252 operations declare this header as required
  description: Global API key used to verify and authorize access to the OpenAPI. Documented as a 35-character string, created under Project Settings -> Basic Settings -> API Key Management. The key is bound to BOTH an account and a project, and inherits exactly the permissions of the account it was issued to.
  id: api-key
  in: header
  lifecycle: Keys are created, listed and revoked in the console; an expired key can no longer be copied. No published rotation interval.
  name: api-key
  required: true
  type: apiKey
- coverage: 252 of 252 operations declare this header as required
  description: Project (tenant) selector. Not a credential on its own, but required on every call and enforced together with the api-key, which is itself project-bound. Example value "default".
  id: sensorsdata-project
  in: header
  name: sensorsdata-project
  required: true
  type: apiKey
- description: Impersonation header. When present, the call executes as the named account — permissions and audit-log attribution follow that account. Documented as usable ONLY with an administrator API key.
  id: account-id
  in: header
  name: account-id
  note: documented in the authentication guide; not present as a parameter in the specs
  required: false
  type: apiKey
- coverage: 70 of 252 operations declare this header
  description: Organization selector on multi-organization deployments.
  id: X-Organization-Id
  in: header
  name: X-Organization-Id
  required: false
  type: apiKey
slug: sensors-data-authentication
source_filename: sensors-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.sensorsdata.com/sa/docs/open_api_authentication\ndocs: https://docs.sensorsdata.com/sa/docs/open_api_authentication\nsummary: >-\n  Every Sensors Data OpenAPI operation is authenticated with a project-scoped API key\n  carried in the api-key request header, alongside a sensorsdata-project header that\n  selects the tenant project. The published specs do not declare a securitySchemes block;\n  the credentials appear as required header parameters on all 252 operations, which is\n  why this profile is written from the authentication documentation rather than derived.\nschemes:\n  - id: api-key\n    type: apiKey\n    in: header\n    name: api-key\n    required: true\n    description: >-\n      Global API key used to verify and authorize access to the OpenAPI. Documented as a\n      35-character string, created under Project Settings -> Basic Settings -> API Key\n      Management. The key is bound to BOTH an account\
  \ and a project, and inherits exactly\n      the permissions of the account it was issued to.\n    lifecycle: >-\n      Keys are created, listed and revoked in the console; an expired key can no longer be\n      copied. No published rotation interval.\n    coverage: 252 of 252 operations declare this header as required\n  - id: sensorsdata-project\n    type: apiKey\n    in: header\n    name: sensorsdata-project\n    required: true\n    description: >-\n      Project (tenant) selector. Not a credential on its own, but required on every call\n      and enforced together with the api-key, which is itself project-bound. Example value\n      \"default\".\n    coverage: 252 of 252 operations declare this header as required\n  - id: account-id\n    type: apiKey\n    in: header\n    name: account-id\n    required: false\n    description: >-\n      Impersonation header. When present, the call executes as the named account —\n      permissions and audit-log attribution follow that account. Documented\
  \ as usable ONLY\n      with an administrator API key.\n    note: documented in the authentication guide; not present as a parameter in the specs\n  - id: X-Organization-Id\n    type: apiKey\n    in: header\n    name: X-Organization-Id\n    required: false\n    description: Organization selector on multi-organization deployments.\n    coverage: 70 of 252 operations declare this header\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes:\n  - >-\n    OAuth 2.0 at Sensors Data is console SSO for human operators (third-party login,\n    documented at /sa/docs/tech_super_three_oauth), not an OpenAPI authorization grant.\n    There are no API OAuth scopes to catalog, so no scopes artifact is published.\n  - >-\n    Legacy pre-v3 query interfaces additionally accept an API_SECRET or a simulated\n    username/password login; the v3 OpenAPI surface documented here is api-key only.\n  - >-\n    Transport is whatever the customer's cluster ingress terminates — the docs state\n    \"\
  HTTP or HTTPS depends on the load balancing configuration at the cluster entrance\",\n    so TLS is a deployment choice, not a platform guarantee.\nexamples:\n  - >-\n    curl -XGET \"http://{host}:8107/api/v3/analytics/v1/project/list\"\n    -H \"Accept: application/json\" -H \"Content-Type: application/json\"\n    -H \"sensorsdata-project: default\" -H \"api-key: {api-key}\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensors-data/refs/heads/main/authentication/sensors-data-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Enterprise
- Analytics
- Customer Data Platform
- Product Analytics
- Data Collection
- SDK
- Marketing
---
