---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Animal And Plant Health Inspection Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Animal and Plant Health Inspection Service declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Animal and Plant Health Inspection Service
provider_slug: animal-and-plant-health-inspection-service
scheme_count: 4
schemes:
- applies_to: APHIS eFile Permitting System
  authorization_endpoint: https://efile.aphis.usda.gov/services/oauth2/authorize
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  end_session_endpoint: https://efile.aphis.usda.gov/services/auth/idp/oidc/logout
  grant_types:
  - authorization_code
  - implicit
  id: oidc-efile
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://efile.aphis.usda.gov/services/oauth2/introspect
  issuer: https://efile.aphis.usda.gov
  jwks_uri: https://efile.aphis.usda.gov/id/keys
  note: Client registration is not open. USDA eAuthentication account required; the registration_endpoint is the Salesforce platform default and is not documented by APHIS as a public onboarding path.
  openIdConnectUrl: https://efile.aphis.usda.gov/.well-known/openid-configuration
  registration_endpoint: https://efile.aphis.usda.gov/services/oauth2/register
  response_types_supported:
  - code
  - token
  - token id_token
  revocation_endpoint: https://efile.aphis.usda.gov/services/oauth2/revoke
  scope_count: 36
  subject_types_supported:
  - public
  token_endpoint: https://efile.aphis.usda.gov/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://efile.aphis.usda.gov/services/oauth2/userinfo
- applies_to: Agricultural Commodity Import Requirements (ACIR)
  authorization_endpoint: https://acir.aphis.usda.gov/services/oauth2/authorize
  id: oidc-acir
  issuer: https://acir.aphis.usda.gov
  jwks_uri: https://acir.aphis.usda.gov/id/keys
  note: ACIR search itself is browsable without sign-in; the OIDC surface backs authenticated features.
  openIdConnectUrl: https://acir.aphis.usda.gov/.well-known/openid-configuration
  scope_count: 36
  token_endpoint: https://acir.aphis.usda.gov/services/oauth2/token
  type: openIdConnect
- applies_to: APHIS Public Search Tool (Animal Care)
  authorization_endpoint: https://aphis.my.site.com/services/oauth2/authorize
  id: oidc-public-search
  issuer: https://aphis.my.site.com
  jwks_uri: https://aphis.my.site.com/id/keys
  openIdConnectUrl: https://aphis.my.site.com/.well-known/openid-configuration
  scope_count: 36
  token_endpoint: https://aphis.my.site.com/services/oauth2/token
  type: openIdConnect
- applies_to: USDA-MRP ArcGIS REST Feature Services
  id: anonymous-arcgis
  note: The 93 public feature services under https://services7.arcgis.com/2C1NQ7u6M6SXoa8p/arcgis/rest/services answer unauthenticated GET/query. No token, key, or referrer restriction was observed on probe. Services declare capabilities Query (a few also Extract) - read-only.
  probe_status: 200
  probed: '2026-09-02'
  type: none
slug: animal-and-plant-health-inspection-service-authentication
source_filename: animal-and-plant-health-inspection-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://efile.aphis.usda.gov/.well-known/openid-configuration (HTTP 200),\n  https://acir.aphis.usda.gov/.well-known/openid-configuration (HTTP 200),\n  https://aphis.my.site.com/.well-known/openid-configuration (HTTP 200),\n  plus https://www.aphis.usda.gov/efile/help (USDA eAuthentication requirement)\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Animal and Plant Health Inspection Service\nproviderId: animal-and-plant-health-inspection-service\ndocs: https://www.eauth.usda.gov/eauth/b/usda/faq\nsummary: >-\n  APHIS publishes no developer API with its own key-issuance flow. Every APHIS digital\n  service that carries an identity boundary authenticates through USDA eAuthentication,\n  federated into the Salesforce Experience Cloud tenants that host APHIS eFile, ACIR and\n  the Animal Care Public Search Tool. Each of those three hosts serves a live OpenID\n  Connect Discovery 1.0 document\
  \ whose issuer is the APHIS host itself, so an OIDC/OAuth 2.0\n  authorization-code surface is measurably present - but it is a platform sign-in surface\n  for the web applications, not a documented developer API. The one genuinely anonymous\n  machine-readable surface APHIS operates, the USDA-MRP ArcGIS REST feature services,\n  requires no authentication at all for read/query.\nschemes:\n  - id: oidc-efile\n    type: openIdConnect\n    applies_to: APHIS eFile Permitting System\n    openIdConnectUrl: https://efile.aphis.usda.gov/.well-known/openid-configuration\n    issuer: https://efile.aphis.usda.gov\n    authorization_endpoint: https://efile.aphis.usda.gov/services/oauth2/authorize\n    token_endpoint: https://efile.aphis.usda.gov/services/oauth2/token\n    userinfo_endpoint: https://efile.aphis.usda.gov/services/oauth2/userinfo\n    jwks_uri: https://efile.aphis.usda.gov/id/keys\n    revocation_endpoint: https://efile.aphis.usda.gov/services/oauth2/revoke\n    introspection_endpoint:\
  \ https://efile.aphis.usda.gov/services/oauth2/introspect\n    registration_endpoint: https://efile.aphis.usda.gov/services/oauth2/register\n    end_session_endpoint: https://efile.aphis.usda.gov/services/auth/idp/oidc/logout\n    grant_types:\n      - authorization_code\n      - implicit\n    response_types_supported:\n      - code\n      - token\n      - token id_token\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    id_token_signing_alg_values_supported:\n      - RS256\n    dpop_signing_alg_values_supported:\n      - RS256\n      - RS384\n      - RS512\n      - ES256\n      - ES384\n      - ES512\n      - EdDSA\n    subject_types_supported:\n      - public\n    scope_count: 36\n    note: >-\n      Client registration is not open. USDA eAuthentication account required; the\n      registration_endpoint is the Salesforce platform default and is not documented by\n      APHIS as a public onboarding path.\n\
  \  - id: oidc-acir\n    type: openIdConnect\n    applies_to: Agricultural Commodity Import Requirements (ACIR)\n    openIdConnectUrl: https://acir.aphis.usda.gov/.well-known/openid-configuration\n    issuer: https://acir.aphis.usda.gov\n    authorization_endpoint: https://acir.aphis.usda.gov/services/oauth2/authorize\n    token_endpoint: https://acir.aphis.usda.gov/services/oauth2/token\n    jwks_uri: https://acir.aphis.usda.gov/id/keys\n    scope_count: 36\n    note: ACIR search itself is browsable without sign-in; the OIDC surface backs authenticated features.\n  - id: oidc-public-search\n    type: openIdConnect\n    applies_to: APHIS Public Search Tool (Animal Care)\n    openIdConnectUrl: https://aphis.my.site.com/.well-known/openid-configuration\n    issuer: https://aphis.my.site.com\n    authorization_endpoint: https://aphis.my.site.com/services/oauth2/authorize\n    token_endpoint: https://aphis.my.site.com/services/oauth2/token\n    jwks_uri: https://aphis.my.site.com/id/keys\n\
  \    scope_count: 36\n  - id: anonymous-arcgis\n    type: none\n    applies_to: USDA-MRP ArcGIS REST Feature Services\n    note: >-\n      The 93 public feature services under\n      https://services7.arcgis.com/2C1NQ7u6M6SXoa8p/arcgis/rest/services answer\n      unauthenticated GET/query. No token, key, or referrer restriction was observed on\n      probe. Services declare capabilities Query (a few also Extract) - read-only.\n    probed: '2026-09-02'\n    probe_status: 200\nidentity_provider:\n  name: USDA eAuthentication\n  url: https://www.eauth.usda.gov/home\n  registration: https://www.eauth.usda.gov/eauth/b/usda/registration\n  faq: https://www.eauth.usda.gov/eauth/b/usda/faq\n  note: >-\n    Level 2 verified eAuthentication account is the prerequisite for APHIS eFile, VSPS,\n    VEHCS and PCIT. Identity proofing is a government process, not a self-service developer\n    signup.\ngaps:\n  - No developer-facing API key issuance or client-credentials flow is documented anywhere on\
  \ aphis.usda.gov.\n  - No documented scope reference; the 36 scopes on the discovery documents are Salesforce platform defaults, not an APHIS-authored permission model.\n  - No machine-readable contract (OpenAPI/GraphQL/WSDL/gRPC) exists to bind these schemes to operations.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/animal-and-plant-health-inspection-service/refs/heads/main/authentication/animal-and-plant-health-inspection-service-authentication.yml
summary_line: 4 schemes
tags:
- Agriculture
- Animal Health
- Animal Welfare
- Biotechnology
- Federal-Government
- Import Export
- Permits
- Pest Control
- Plant Health
- Regulatory
- USDA
- Wildlife
---
