---
api_key_in: []
api_specs:
- filename: sertica-web-api-openapi.json
  format: json
  label: SERTICA Web API
  slug: sertica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/openapi/sertica-web-api-openapi.json
auth_types:
- http
description: SERTICA Web API authentication. The spec declares a single HTTP bearer scheme; the provider's own support documentation supplies the token-issuing flow, the lifetime, and the per-user authorization model that the spec expresses only as prose inside each operation's 403 response description.
kind: authentication
layout: security
method: searched
name: Sertica Authentication
name_suffix: Authentication
oauth_flows: []
overview: SERTICA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SERTICA
provider_slug: sertica
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT Authorization header using the Bearer scheme
  name: Bearer
  scheme: bearer
  sources:
  - openapi/sertica-web-api-openapi.json
  type: http
slug: sertica-authentication
source_filename: sertica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/sertica-web-api-openapi.json\ndocs: https://support.sertica.com/hc/en-us/articles/28558470734109-SERTICA-Application-Programming-Interface\ndescription: >-\n  SERTICA Web API authentication. The spec declares a single HTTP bearer scheme; the\n  provider's own support documentation supplies the token-issuing flow, the lifetime, and\n  the per-user authorization model that the spec expresses only as prose inside each\n  operation's 403 response description.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Authorization header using the Bearer scheme\n  sources:\n  - openapi/sertica-web-api-openapi.json\ntoken_issuance:\n  operation: CreateJwtToken\n  method: POST\n  path: /Auth\n  request_body:\n    login: string\n    password: string\n  response_field: accessToken\n  header: 'Authorization: Bearer <accessToken>'\n\
  \  lifetime: 24 hours (provider-stated default)\n  lifetime_source: https://support.sertica.com/hc/en-us/articles/28558470734109-SERTICA-Application-Programming-Interface\n  note: >-\n    A second token operation, CreateAccessToken (POST /Auth/accessToken), is declared in\n    the spec without a summary; the support article documents only POST /Auth. A separate\n    short-lived download token is issued by GET /Auth/fileDownloadToken.\nmulti_factor:\n  supported: true\n  mechanism: TOTP authenticator app\n  operations:\n  - SetupTotp\n  - ConfirmTotpSetup\n  - GenerateRecoveryCodes\n  - DisableTotp\n  introduced: Ver 5.15.89 (2025-11-17)\n  source: https://support.sertica.com/hc/en-us/articles/31855511177757-Ver-5-15-89\nauthorization_model:\n  style: per-user rights, evaluated per operation\n  description: >-\n    Every request is bound to a SERTICA user, and a caller sees only the data that user\n    can see. 3,028 of 3,340 operations declare a 403 whose description names the exact\n\
  \    User Right key required (for example \"AnalyticsMain / View\", \"ChangeRequest / View\").\n    This is a real, machine-extractable permission surface, but it is carried in prose\n    inside response descriptions rather than in OAuth scopes.\n  discovery_operations:\n  - Get list of valid user rights for the user   # GET /Auth/userRights\n  - Get list of roles assigned to user           # GET /Auth/{login}/roles\n  - Get List of Units current user has access to # GET /Auth/units\n  oauth2: false\n  scopes: none\nexternal_identity:\n  operation: AuthIntegrations\n  path: /Auth/integrations\n  note: >-\n    Returns the configured Authentication Integrations for the site. The spec does not\n    enumerate the supported providers and the public docs do not document them, so the\n    set of external identity providers is site-specific and not stated here.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/authentication/sertica-authentication.yml
summary_line: http · 1 scheme
tags:
- Maritime
- Shipping
- Fleet Management
- Maintenance
- Procurement
- Asset Management
- Compliance
- Enterprise Software
---
