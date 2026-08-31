---
api_key_in: []
auth_types: []
description: 'Troy Medicare publishes no public developer portal and no OpenAPI, so this profile is derived entirely from the two OpenID Connect discovery documents its own hosts serve anonymously. Both are OAuth 2.0 authorization servers: one in front of the secure provider portal, one in front of the health plan''s FHIR data surface. Neither documents client registration publicly — a third-party application developer has no published path to credentials.'
kind: authentication
layout: security
method: probed
name: Troy Medicare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Troy Medicare declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Troy Medicare
provider_slug: troy-medicare
scheme_count: 2
schemes:
- authorization_endpoint: https://provider.troymedicare.com/connect/authorize
  device_authorization_endpoint: https://provider.troymedicare.com/connect/deviceauthorization
  end_session_endpoint: https://provider.troymedicare.com/connect/endsession
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - LinkLogin
  - Impersonation
  host: provider.troymedicare.com
  id: provider-portal-oidc
  id_token_signing_alg_values:
  - RS256
  introspection_endpoint: https://provider.troymedicare.com/connect/introspect
  issuer: https://provider.troymedicare.com
  jwks_uri: https://provider.troymedicare.com/.well-known/openid-configuration/jwks
  logout:
    backchannel: true
    frontchannel: true
  notes:
  - Two non-standard grant types are advertised — `LinkLogin` and `Impersonation` — alongside the legacy `password` and `implicit` grants. Both legacy grants are discouraged by OAuth 2.0 Security BCP (RFC 9700) / OAuth 2.1.
  - Scope and claim names (NirvanaHealth, NhCore, nh_web_resource, nh_pcmweb_resource, DMR, M3P, ClaimCore) identify the underlying platform as NirvanaHealth's Aria, which Troy Medicare announced it selected in July 2023 (https://troymedicare.com/press/2023-07/troy-medicare-selects-nirvanahealth-aria-platform). The authorization server is nonetheless issued and hosted under Troy Medicare's own domain and issuer identifier.
  openIdConnectUrl: https://provider.troymedicare.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  response_modes:
  - form_post
  - query
  - fragment
  response_types:
  - code
  - token
  - id_token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  revocation_endpoint: https://provider.troymedicare.com/connect/revocation
  scope_count: 35
  scopes_file: scopes/troy-medicare-scopes.yml
  token_endpoint: https://provider.troymedicare.com/connect/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://provider.troymedicare.com/connect/userinfo
- authorization_endpoint: https://fhir.troymedicare.com/oauth/authorization
  host: fhir.troymedicare.com
  id: fhir-oauth
  id_token_signing_alg_values:
  - RS256
  issuer: https://fhir.troymedicare.com
  jwks_uri: https://fhir.troymedicare.com/.well-known/jwk
  notes:
  - The discovery document omits scopes_supported, grant_types_supported, userinfo_endpoint and token_endpoint_auth_methods_supported, so the SMART on FHIR scope vocabulary this surface accepts cannot be read anonymously.
  - GET /oauth/authorization without parameters 302s to the host root, which serves a Troy-Medicare-branded username/password sign-in page — consistent with a member-authorization (consent) front door rather than a developer console.
  - No /.well-known/smart-configuration is served and no CapabilityStatement was reachable at any probed path, so the FHIR release, resource set and SMART capabilities are unverified.
  openIdConnectUrl: https://fhir.troymedicare.com/.well-known/openid-configuration
  response_types:
  - code
  - id_token
  - token id_token
  scopes_advertised: none
  subject_types:
  - pairwise
  - public
  token_endpoint: https://fhir.troymedicare.com/oauth/token
  type: oauth2
slug: troy-medicare-authentication
source_filename: troy-medicare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Troy Medicare Authentication\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://provider.troymedicare.com/.well-known/openid-configuration (HTTP 200) and\n  https://fhir.troymedicare.com/.well-known/openid-configuration (HTTP 200), fetched 2026-08-30.\ndescription: >-\n  Troy Medicare publishes no public developer portal and no OpenAPI, so this profile is derived\n  entirely from the two OpenID Connect discovery documents its own hosts serve anonymously. Both\n  are OAuth 2.0 authorization servers: one in front of the secure provider portal, one in front of\n  the health plan's FHIR data surface. Neither documents client registration publicly — a\n  third-party application developer has no published path to credentials.\nschemes:\n- id: provider-portal-oidc\n  type: openIdConnect\n  host: provider.troymedicare.com\n  issuer: https://provider.troymedicare.com\n  openIdConnectUrl: https://provider.troymedicare.com/.well-known/openid-configuration\n  authorization_endpoint:\
  \ https://provider.troymedicare.com/connect/authorize\n  token_endpoint: https://provider.troymedicare.com/connect/token\n  userinfo_endpoint: https://provider.troymedicare.com/connect/userinfo\n  jwks_uri: https://provider.troymedicare.com/.well-known/openid-configuration/jwks\n  introspection_endpoint: https://provider.troymedicare.com/connect/introspect\n  revocation_endpoint: https://provider.troymedicare.com/connect/revocation\n  end_session_endpoint: https://provider.troymedicare.com/connect/endsession\n  device_authorization_endpoint: https://provider.troymedicare.com/connect/deviceauthorization\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - LinkLogin\n  - Impersonation\n  response_types: [code, token, id_token, id_token token, code id_token, code token, code id_token token]\n  response_modes: [form_post, query, fragment]\n  token_endpoint_auth_methods: [client_secret_basic,\
  \ client_secret_post]\n  id_token_signing_alg_values: [RS256]\n  pkce:\n    supported: true\n    code_challenge_methods: [plain, S256]\n  logout:\n    frontchannel: true\n    backchannel: true\n  scope_count: 35\n  scopes_file: scopes/troy-medicare-scopes.yml\n  notes:\n  - >-\n    Two non-standard grant types are advertised — `LinkLogin` and `Impersonation` — alongside the\n    legacy `password` and `implicit` grants. Both legacy grants are discouraged by OAuth 2.0\n    Security BCP (RFC 9700) / OAuth 2.1.\n  - >-\n    Scope and claim names (NirvanaHealth, NhCore, nh_web_resource, nh_pcmweb_resource, DMR, M3P,\n    ClaimCore) identify the underlying platform as NirvanaHealth's Aria, which Troy Medicare\n    announced it selected in July 2023 (https://troymedicare.com/press/2023-07/troy-medicare-selects-nirvanahealth-aria-platform).\n    The authorization server is nonetheless issued and hosted under Troy Medicare's own domain and\n    issuer identifier.\n- id: fhir-oauth\n  type: oauth2\n\
  \  host: fhir.troymedicare.com\n  issuer: https://fhir.troymedicare.com\n  openIdConnectUrl: https://fhir.troymedicare.com/.well-known/openid-configuration\n  authorization_endpoint: https://fhir.troymedicare.com/oauth/authorization\n  token_endpoint: https://fhir.troymedicare.com/oauth/token\n  jwks_uri: https://fhir.troymedicare.com/.well-known/jwk\n  response_types: [code, id_token, token id_token]\n  subject_types: [pairwise, public]\n  id_token_signing_alg_values: [RS256]\n  scopes_advertised: none\n  notes:\n  - >-\n    The discovery document omits scopes_supported, grant_types_supported, userinfo_endpoint and\n    token_endpoint_auth_methods_supported, so the SMART on FHIR scope vocabulary this surface\n    accepts cannot be read anonymously.\n  - >-\n    GET /oauth/authorization without parameters 302s to the host root, which serves a\n    Troy-Medicare-branded username/password sign-in page — consistent with a member-authorization\n    (consent) front door rather than a developer\
  \ console.\n  - >-\n    No /.well-known/smart-configuration is served and no CapabilityStatement was reachable at any\n    probed path, so the FHIR release, resource set and SMART capabilities are unverified.\nclient_registration:\n  public_documentation: none\n  dynamic_registration: not-advertised\n  note: >-\n    Neither host advertises RFC 7591 dynamic client registration, and no application-registration\n    or developer-onboarding page was found on troymedicare.com (sitemap.xml enumerates 55 URLs,\n    none of them developer-facing).\nevidence:\n- url: https://provider.troymedicare.com/.well-known/openid-configuration\n  status: 200\n- url: https://fhir.troymedicare.com/.well-known/openid-configuration\n  status: 200\n- url: https://fhir.troymedicare.com/.well-known/jwk\n  status: 200\n- url: https://fhir.troymedicare.com/oauth/authorization\n  status: 302\n- url: https://fhir.troymedicare.com/.well-known/smart-configuration\n  status: 404\n- url: https://fhir.troymedicare.com/metadata\n\
  \  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/troy-medicare/refs/heads/main/authentication/troy-medicare-authentication.yml
summary_line: 2 schemes
tags:
- Health Insurance
- Medicare
- Medicare Advantage
- Health Plans
- Healthcare
- Pharmacy
- Care Management
- Insurance
- Identity
- OpenID Connect
---
