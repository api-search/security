---
api_key_in: []
api_specs:
- filename: tuva-health-config-api-openapi.yml
  format: yaml
  label: Tuva Health Config API
  slug: tuva-health-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-config-api-openapi.yml
- filename: tuva-health-data-sources-api-openapi.yml
  format: yaml
  label: Tuva Health Data Sources API
  slug: tuva-health-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-data-sources-api-openapi.yml
- filename: tuva-health-health-check-api-openapi.yml
  format: yaml
  label: Tuva Health Health Check API
  slug: tuva-health-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-health-check-api-openapi.yml
- filename: tuva-health-matches-api-openapi.yml
  format: yaml
  label: Tuva Health Matches API
  slug: tuva-health-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-matches-api-openapi.yml
- filename: tuva-health-person-records-api-openapi.yml
  format: yaml
  label: Tuva Health Person Records API
  slug: tuva-health-person-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-person-records-api-openapi.yml
- filename: tuva-health-persons-api-openapi.yml
  format: yaml
  label: Tuva Health Persons API
  slug: tuva-health-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-persons-api-openapi.yml
- filename: tuva-health-potential-matches-api-openapi.yml
  format: yaml
  label: Tuva Health Potential Matches API
  slug: tuva-health-potential-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-potential-matches-api-openapi.yml
- filename: tuva-health-users-api-openapi.yml
  format: yaml
  label: Tuva Health Users API
  slug: tuva-health-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/openapi/tuva-health-users-api-openapi.yml
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tuva Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tuva Health secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tuva Health
provider_slug: tuva-health
scheme_count: 1
schemes:
- description: A JWT issued by the customer's identity provider, forwarded to the API by the authenticating proxy on the header named by idp.<backend>.jwt_header (default X-Forwarded-Access-Token). The backend verifies the token against the configured JWKS URL, client ID and audience claim.
  documented_in: docs
  header: X-Forwarded-Access-Token
  header_configurable: true
  identity_providers:
  - config_key: idp.keycloak
    id: keycloak
    settings:
    - server_url
    - realm
    - jwt_header
    - jwt_aud
    - jwks_url
    - client_id
    - client_secret
  - config_key: idp.aws_cognito
    id: aws-cognito
    settings:
    - cognito_user_pool_id
    - jwt_header
    - jwks_url
    - client_id
  name: oidc-jwt-forwarded-header
  sources:
  - https://tuva-health.github.io/tuva_empi/docs/configuration
  type: openIdConnect
slug: tuva-health-authentication
source_filename: tuva-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: openapi/tuva-health-empi-openapi.yml\ndocs: https://tuva-health.github.io/tuva_empi/docs/configuration\nnote: >-\n  Derived mechanically first (0-working/derive-authentication.py returned zero\n  profiles: the published Tuva EMPI OpenAPI declares NO components.securitySchemes\n  and no top-level security requirement, so the spec is silent on auth). Upgraded\n  to `searched` from the provider's own configuration documentation, which does\n  document the real model: Tuva EMPI is deployed behind an OAuth2/OIDC reverse\n  proxy (oauth2-proxy in the reference Docker Compose stack) and the Django\n  backend validates a JWT presented on a configurable header. Because Tuva EMPI\n  is customer-deployed software, the identity provider, issuer, JWKS URL, client\n  ID and audience are all CUSTOMER-supplied configuration - Tuva operates no\n  authorization server of its own.\nsummary:\n  types: [openIdConnect]\n  api_key_in: []\n  oauth2_flows:\
  \ []\n  token_transport: http-header\n  spec_declares_security: false\nschemes:\n  - name: oidc-jwt-forwarded-header\n    type: openIdConnect\n    documented_in: docs\n    sources: [https://tuva-health.github.io/tuva_empi/docs/configuration]\n    header: X-Forwarded-Access-Token\n    header_configurable: true\n    description: >-\n      A JWT issued by the customer's identity provider, forwarded to the API by\n      the authenticating proxy on the header named by idp.<backend>.jwt_header\n      (default X-Forwarded-Access-Token). The backend verifies the token against\n      the configured JWKS URL, client ID and audience claim.\n    identity_providers:\n      - id: keycloak\n        config_key: idp.keycloak\n        settings: [server_url, realm, jwt_header, jwt_aud, jwks_url, client_id, client_secret]\n      - id: aws-cognito\n        config_key: idp.aws_cognito\n        settings: [cognito_user_pool_id, jwt_header, jwks_url, client_id]\nauthorization:\n  model: role-based\n  note: >-\n\
  \    Roles are held in Tuva EMPI itself (components.schemas.RoleEnum in the\n    OpenAPI) and updated through POST /api/v1/users/{id}\n    (operationId users_create). The first admin is granted at bootstrap time\n    from initial_setup.admin_email, which must already exist in the external\n    identity provider.\n  roles_source: openapi/tuva-health-empi-openapi.yml#/components/schemas/RoleEnum\nscopes: []\ngaps:\n  - >-\n    The published OpenAPI declares no securitySchemes and applies no security to\n    any of its 12 operations, so a generated client or agent reading the contract\n    alone would believe the API is unauthenticated. Declaring an\n    openIdConnect / http-bearer scheme in the spec would close this.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/authentication/tuva-health-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Healthcare
- United States
- Health Data
- FHIR
- Interoperability
- Data Analytics
- Data Transformation
- Claims
- Open-Source
- dbt
- EMPI
- Patient Matching
---
