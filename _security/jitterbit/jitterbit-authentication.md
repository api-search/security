---
api_key_in:
- header
api_specs:
- filename: jitterbit-login-api-openapi.yml
  format: yaml
  label: Jitterbit Login API
  slug: jitterbit-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-login-api-openapi.yml
- filename: jitterbit-operations-api-openapi.yml
  format: yaml
  label: Jitterbit Operations API
  slug: jitterbit-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-operations-api-openapi.yml
- filename: jitterbit-projects-api-openapi.yml
  format: yaml
  label: Jitterbit Projects API
  slug: jitterbit-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-projects-api-openapi.yml
- filename: jitterbit-schedules-api-openapi.yml
  format: yaml
  label: Jitterbit Schedules API
  slug: jitterbit-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-schedules-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Jitterbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jitterbit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jitterbit
provider_slug: jitterbit
scheme_count: 1
schemes:
- applied_to: 17 of 19 operations (all except POST /login and GET /login)
  description: 'An opaque Harmony session token passed in the authToken request header. Observed format in published examples: 1_<uuid>. The Cloud RESTful Service login response reports sessionTimeoutInSeconds 14400 (4 hours).'
  in: header
  name: authToken
  parameter: authToken
  sources:
  - openapi/jitterbit-harmony-platform-openapi.yml
  type: apiKey
slug: jitterbit-authentication
source_filename: jitterbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/jitterbit-harmony-platform-openapi.yml\ndocs: https://developer.jitterbit.com/harmony-platform-apis/\nadditional_docs:\n  - https://docs.jitterbit.com/developer-portal/connector-sdk/apis/\n  - https://docs.jitterbit.com/api-manager/api-manager-reference/api-manager-log-service-api/\n  - https://docs.jitterbit.com/getting-started/jitterbit-security/sso/\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: authToken\n    type: apiKey\n    in: header\n    parameter: authToken\n    sources:\n      - openapi/jitterbit-harmony-platform-openapi.yml\n    applied_to: 17 of 19 operations (all except POST /login and GET /login)\n    description: >-\n      An opaque Harmony session token passed in the authToken request header.\n      Observed format in published examples: 1_<uuid>. The Cloud RESTful Service\n      login response reports\
  \ sessionTimeoutInSeconds 14400 (4 hours).\ntoken_acquisition:\n  - surface: Harmony platform API\n    operation: authenticate\n    method: POST\n    path: /login\n    parameters: [username, password]\n    passed_as: query parameters\n    returns: authenticationToken\n    caveat: >-\n      \"The username and password must be associated with Harmony account\n      credentials and not an organization using Harmony SSO.\" An SSO-only\n      organization cannot obtain a token through this operation.\n  - surface: Jitterbit Cloud RESTful Service (User Service Controller API)\n    method: PUT\n    path: /jitterbit-cloud-restful-service/user/login\n    body: '{\"email\": \"...\", \"password\": \"...\"}'\n    content_type: application/json\n    returns: 'authenticationToken, serverUrl, cloudAppsUrl, orgAttrs[], defaultOrgId, sessionTimeoutInSeconds'\n    role_requirement: A user with Admin permission in the organization is required for the API Manager Log Service API.\n  - surface: Jitterbit Cloud\
  \ RESTful Service — two-factor\n    method: PUT\n    path: /jitterbit-cloud-restful-service/user/login/tfacode\n    flow: >-\n      When the organization has TFA enabled, the plain login fails with\n      errorCode VALIDATE_TFA_LOGIN_EMAIL and emails a code. A second request\n      carrying email, password, code and deviceId returns the token.\n    body_fields: [email, password, code, deviceId]\ntoken_conversion:\n  operation: convertAuthtokenToJwt\n  method: GET\n  path: /login\n  parameter: authToken\n  returns: JSON Web Token\n  status: >-\n    Declared in the contract but described there as \"handled automatically for\n    the user where appropriate and currently has no application.\"\nregions:\n  harmony_platform_api:\n    - https://harmony-api.na-east.jitterbit.com/{endpoint}\n    - https://harmony-api.emea-west.jitterbit.com/{endpoint}\n    - https://harmony-api.apac-southeast.jitterbit.com/{endpoint}\n  cloud_restful_service:\n    NA: https://na-east.jitterbit.com/jitterbit-cloud-restful-service/\n\
  \    EMEA: https://emea-west.jitterbit.com/jitterbit-cloud-restful-service/\n    APAC: https://apac-southeast.jitterbit.com/jitterbit-cloud-restful-service/\n  note: >-\n    A token is bound to a region. The organization's region determines the host;\n    Finding My Region is the documented way to establish it.\nplatform_authentication:\n  note: >-\n    Distinct from the API above. These are the authentication mechanisms\n    Jitterbit gives to the APIs its CUSTOMERS publish through API Manager, and\n    to Harmony platform login.\n  harmony_login:\n    - password with configurable policy (special-character requirement, TFA requirement)\n    - two-factor authentication by emailed code\n    - 'single sign-on via SAML 2.0 or OAuth 2.0 against an external identity provider (docs: https://docs.jitterbit.com/getting-started/jitterbit-security/sso/)'\n    - security question and answer as an additional identity verification (12.8)\n  customer_api_security_profiles:\n    - anonymous\n    - basic\n\
  \    - api-key\n    - 'OAuth 2.0 two-legged (Microsoft Entra ID / Azure AD, Okta)'\n    - 'OAuth 2.0 three-legged (Microsoft Entra ID / Azure AD, Okta, Google, Salesforce)'\n    - JWT\n    - trusted IP groups (network-level restriction, rejects with 429)\n  api_key_expiry:\n    since: '12.9'\n    default_days: 180\n    behavior: >-\n      An API key security profile can be configured to expire; requests using an\n      expired key are rejected. An Expiring soon pill appears within 7 days and a\n      reminder email goes to organization administrators. The cloud API gateway\n      enforces expiry automatically; a private API gateway requires 12.9 or later.\n  credential_masking:\n    since: '12.9'\n    behavior: 'Header values carrying credentials or session data (authorization, password, x_api_key) are replaced with [removed] in API logs.'\ngaps:\n  - No OAuth 2.0, OIDC or scoped authorization for Jitterbit's own APIs — a single all-or-nothing session token.\n  - Credentials are passed\
  \ as query parameters on the Harmony platform API's POST /login, so they land in URLs and can be logged upstream.\n  - No token refresh or revocation operation is published; the token simply expires after 4 hours.\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any host (all 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/authentication/jitterbit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Management
- Automation
- Integration
- iPaaS
- EDI
- Low-Code
- Enterprise
- API Gateway
- Workflow Automation
- Connectors
---
