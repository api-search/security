---
api_key_in:
- header
api_specs:
- filename: graphiant-portal-openapi-original.json
  format: json
  label: Graphiant Portal REST API
  slug: graphiant-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphiant/refs/heads/main/openapi/graphiant-portal-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Graphiant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphiant secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graphiant
provider_slug: graphiant
scheme_count: 1
schemes:
- applied: 'global root security [{jwtAuth: []}]; 512 of 525 operations also declare an explicit Authorization header parameter'
  description: Use `Bearer <token>` — the token returned by POST /v1/auth/login.
  in: header
  name: jwtAuth
  parameter: authorization
  sources:
  - openapi/graphiant-portal-openapi-original.json
  type: apiKey
  value_format: Bearer <token>
slug: graphiant-authentication
source_filename: graphiant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/graphiant-portal-openapi-original.json\ndocs: https://docs.graphiant.com/docs/graphiant-portal-rest-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: opaque bearer token issued by a username/password (or SAML SSO) login endpoint\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: jwtAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  value_format: Bearer <token>\n  description: Use `Bearer <token>` — the token returned by POST /v1/auth/login.\n  sources: [openapi/graphiant-portal-openapi-original.json]\n  applied: 'global root security [{jwtAuth: []}]; 512 of 525 operations also declare\n    an explicit Authorization header parameter'\ntoken:\n  issuer_endpoint: POST https://api.graphiant.com/v1/auth/login\n  request_body: {username: string, password: string}\n  response_body: {auth: boolean, accountType: msp | enterprise | graphiant, token:\
  \ string}\n  token_format: opaque, prefixed `gr-auth-` followed by two UUIDs\n  lifetime_minutes: 30\n  refresh_endpoint: GET https://api.graphiant.com/v1/auth/refresh\n  refresh_note: accepts the current OR the just-expired token and returns a new one\n  revocation_endpoint: POST https://api.graphiant.com/v1/auth/logout\n  revocation_note: logout immediately invalidates the token; subsequent calls return\n    errorCode 403 \"Invalid Token\"\n  header: 'authorization: Bearer <token>'\nlogin_methods:\n- method: local password\n  endpoint: POST /v1/auth/login\n- method: SAML SSO\n  endpoint: GET /v1/auth/login/saml\n  docs: https://docs.graphiant.com/docs/sso-setup-using-okta-saml\n  note: Okta SAML documented as the reference identity provider\n- method: MFA\n  endpoint: POST /v1/auth/mfa\n  docs: https://docs.graphiant.com/docs/multi-factor-authentification-mfa\n  note: SMS or Google Authenticator, configured per user in the Graphiant Portal\nmulti_tenancy:\n  model: MSP over enterprise\
  \ tenants\n  account_types: [msp, enterprise, graphiant]\n  whoami_endpoint: GET /v1/auth/user\n  list_tenants_endpoint: GET /v1/enterprises\n  user_tenants_endpoint: GET /v1/users/{userId}/enterprises\n  impersonate_endpoint: GET /v1/auth/session?enterpriseId={id}\n  return_to_root_endpoint: GET /v1/auth/session/root\n  note: an MSP user must be explicitly associated with a tenant enterprise; MSP admin\n    status alone does not grant tenant context switching\npermission_domains:\n  note: >-\n    Graphiant does not implement OAuth scopes. Authorization is a per-user permission\n    matrix returned by GET /v1/auth/user, each domain carrying a read or read_write\n    grade. These are the documented domains.\n  values: [assetManager, networkConfiguration, servicePolicies, safetyAndSecurity,\n    globalServices, userAndTenantManagement, insights, reports, monitoringAndTroubleshooting,\n    compliance, logs, developerTools, licensing, billingAndInvoicing, orderStatus,\n    support, gateway,\
  \ b2b]\nsdk_support:\n  environment_variable: GRAPHIANT_ACCESS_TOKEN\n  cli_login: graphiant login (Playwright portal capture) then `source ~/.graphiant/env.sh`\n  credential_store: ~/.graphiant/credentials.json (named profiles)\n  caveat: >-\n    the generated clients warn against setting both Configuration.api_key for jwtAuth\n    and the per-call `authorization` argument — two Authorization headers cause some\n    gateways (for example Azure Application Gateway) to return 400.\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - https://docs.graphiant.com/docs/graphiant-portal-rest-api\n  - https://github.com/Graphiant-Inc/graphiant-sdk-python\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphiant/refs/heads/main/authentication/graphiant-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Networking
- Network as a Service
- NaaS
- Connectivity
- SD-WAN
- Cloud Networking
- Zero Trust
- Network Security
- Data Sovereignty
- Observability
- Infrastructure
- Automation
---
