---
api_key_in: []
api_specs:
- filename: nus-authorization-api-openapi.yml
  format: yaml
  label: National University of Singapore Authorization API
  slug: nus-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-authorization-api-openapi.yml
- filename: nus-discovery-api-openapi.yml
  format: yaml
  label: National University of Singapore Discovery API
  slug: nus-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-discovery-api-openapi.yml
- filename: nus-session-api-openapi.yml
  format: yaml
  label: National University of Singapore Session API
  slug: nus-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-session-api-openapi.yml
auth_types: []
description: Authentication posture across every National University of Singapore surface that could be reached from the open internet. NUS runs one institution-operated authorization server and fronts essentially everything gated with it; the small number of publicly readable surfaces are open metadata endpoints on rented platforms.
kind: authentication
layout: security
method: probed
name: Nus Authentication
name_suffix: Authentication
oauth_flows: []
overview: National University of Singapore declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: National University of Singapore
provider_slug: nus
scheme_count: 4
schemes:
- authorization_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/authorize/
  client_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - windows_client_authentication
  device_authorization_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/devicecode
  discovery: https://vafs.nus.edu.sg/adfs/.well-known/openid-configuration
  end_session_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/logout
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - implicit
  - password
  - srv_challenge
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://vafs.nus.edu.sg/adfs
  jwks_uri: https://vafs.nus.edu.sg/adfs/discovery/keys
  name: NUS federated identity (OpenID Connect / OAuth 2.0)
  onboarding: Relying parties are registered by NUS Information Technology. There is no public dynamic client registration endpoint and no self-service developer signup; a client_id exists only once NUS IT creates one, which in practice requires institutional affiliation.
  pkce_advertised: false
  registration_endpoint_advertised: false
  self_service: false
  subject_type: pairwise
  token_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/token/
  token_signing_algorithms:
  - RS256
  type: openIdConnect
  userinfo_endpoint: https://vafs.nus.edu.sg/adfs/userinfo
  x-operator: institution
- detail: See identity-federation/nus-identity-federation.yml
  entityID: https://vafs.nus.edu.sg/adfs/services/trust
  federation: Singapore Access Federation (SGAF), interfederating with eduGAIN
  metadata: https://vafs.nus.edu.sg/FederationMetadata/2007-06/FederationMetadata.xml
  name: NUS federated identity (SAML 2.0 / WS-Federation / WS-Trust)
  sso_endpoint: https://vafs.nus.edu.sg/adfs/ls/
  type: saml2
  x-operator: institution
- applies_to: https://nnextbus.nus.edu.sg/
  detail: The NUS internal shuttle bus (NextBus) API is live and institution-operated but sits behind HTTP Basic credentials that NUS does not issue publicly. Credentials are not obtainable without affiliation; no probe here attempted to guess or defeat them.
  evidence: 'HTTP/1.1 401 UNAUTHORIZED, WWW-Authenticate: Basic realm="Authentication Required"'
  name: HTTP Basic authentication
  scheme: basic
  type: http
  x-operator: institution
- applies_to:
  - https://scholarbank.nus.edu.sg/server/api
  - https://scholarbank.nus.edu.sg/oai/request
  - https://blog.nus.edu.sg/wp-json/
  detail: Open scholarly and publishing metadata is readable without credentials. All three run on rented platforms (Atmire Open Repository for ScholarBank, CampusPress for Blog.nus), so the absence of authentication is the platform's design decision, not NUS's engineering.
  name: Anonymous read
  type: none
  x-operator: tenant
slug: nus-authentication
source_filename: nus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  https://vafs.nus.edu.sg/adfs/.well-known/openid-configuration (200),\n  https://vafs.nus.edu.sg/adfs/discovery/keys (200),\n  https://vafs.nus.edu.sg/FederationMetadata/2007-06/FederationMetadata.xml (200),\n  https://nnextbus.nus.edu.sg/BusStops (401, WWW-Authenticate: Basic),\n  https://scholarbank.nus.edu.sg/server/api (200, anonymous read) — all fetched 2026-08-19\nprovider: National University of Singapore\nproviderId: nus\ndescription: >-\n  Authentication posture across every National University of Singapore surface that could be\n  reached from the open internet. NUS runs one institution-operated authorization server and\n  fronts essentially everything gated with it; the small number of publicly readable surfaces\n  are open metadata endpoints on rented platforms.\nschemes:\n- name: NUS federated identity (OpenID Connect / OAuth 2.0)\n  type: openIdConnect\n  x-operator: institution\n  issuer: https://vafs.nus.edu.sg/adfs\n\
  \  discovery: https://vafs.nus.edu.sg/adfs/.well-known/openid-configuration\n  jwks_uri: https://vafs.nus.edu.sg/adfs/discovery/keys\n  authorization_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/authorize/\n  token_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/token/\n  userinfo_endpoint: https://vafs.nus.edu.sg/adfs/userinfo\n  end_session_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/logout\n  device_authorization_endpoint: https://vafs.nus.edu.sg/adfs/oauth2/devicecode\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  - implicit\n  - password\n  - srv_challenge\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  client_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - windows_client_authentication\n  token_signing_algorithms:\n  - RS256\n  subject_type: pairwise\n  pkce_advertised: false\n  registration_endpoint_advertised: false\n  self_service: false\n\
  \  onboarding: >-\n    Relying parties are registered by NUS Information Technology. There is no public dynamic\n    client registration endpoint and no self-service developer signup; a client_id exists only\n    once NUS IT creates one, which in practice requires institutional affiliation.\n- name: NUS federated identity (SAML 2.0 / WS-Federation / WS-Trust)\n  type: saml2\n  x-operator: institution\n  entityID: https://vafs.nus.edu.sg/adfs/services/trust\n  metadata: https://vafs.nus.edu.sg/FederationMetadata/2007-06/FederationMetadata.xml\n  sso_endpoint: https://vafs.nus.edu.sg/adfs/ls/\n  federation: Singapore Access Federation (SGAF), interfederating with eduGAIN\n  detail: See identity-federation/nus-identity-federation.yml\n- name: HTTP Basic authentication\n  type: http\n  scheme: basic\n  x-operator: institution\n  applies_to: https://nnextbus.nus.edu.sg/\n  evidence: 'HTTP/1.1 401 UNAUTHORIZED, WWW-Authenticate: Basic realm=\"Authentication Required\"'\n  detail: >-\n    The\
  \ NUS internal shuttle bus (NextBus) API is live and institution-operated but sits behind\n    HTTP Basic credentials that NUS does not issue publicly. Credentials are not obtainable\n    without affiliation; no probe here attempted to guess or defeat them.\n- name: Anonymous read\n  type: none\n  x-operator: tenant\n  applies_to:\n  - https://scholarbank.nus.edu.sg/server/api\n  - https://scholarbank.nus.edu.sg/oai/request\n  - https://blog.nus.edu.sg/wp-json/\n  detail: >-\n    Open scholarly and publishing metadata is readable without credentials. All three run on\n    rented platforms (Atmire Open Repository for ScholarBank, CampusPress for Blog.nus), so the\n    absence of authentication is the platform's design decision, not NUS's engineering.\n\nobservations:\n- >-\n  NUS advertises the `password` and `implicit` grant types, both of which OAuth 2.1 and the\n  IETF security BCP deprecate. This is an ADFS default rather than a deliberate NUS choice, but\n  it is what the institution's\
  \ live discovery document currently tells clients is available.\n- >-\n  PKCE is not advertised in the discovery document. ADFS supports it; the metadata does not\n  declare `code_challenge_methods_supported`, so a conformant client cannot discover it.\n- >-\n  Subject identifiers are pairwise, which means `sub` is per-relying-party. Any agent or\n  integrator expecting a stable cross-application NUS campus identifier will not get one from\n  this provider.\n- >-\n  There is no public developer registration path anywhere in the NUS estate. Every gated NUS\n  API — including the shuttle bus API — is reachable only through an internal request to NUS IT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/authentication/nus-authentication.yml
summary_line: 4 schemes
tags:
- University
- Higher Education
- Education
- Singapore
- Research
- Identity Federation
- Research Repository
- Course Catalog
- Open Access
- Learning Management
---
