---
api_key_in: []
auth_types: []
description: Authentication profile for the Bloomberg Data API surface. Derived from Bloomberg's own published OAuth/OIDC discovery documents rather than from an OpenAPI document — Bloomberg publishes no public machine-readable contract for the Data License REST API, but it does publish RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata, which name the token endpoint, the grant types and the flows exactly.
kind: authentication
layout: security
method: searched
name: Bloomberg Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomberg Data declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Bloomberg Data
provider_slug: bloomberg-data
scheme_count: 3
schemes:
- applies_to:
  - Bloomberg Data License API
  authorization_endpoint: https://bsso.blpprofessional.com/as/authorization.oauth2
  authorization_server: https://bsso.blpprofessional.com
  authorization_server_metadata: https://bsso.blpprofessional.com/.well-known/oauth-authorization-server
  credential_issuance: Client credentials are issued to a contracted Data License customer from the Bloomberg Enterprise Console (console.blpprofessional.com); there is no self-service signup.
  device_authorization_endpoint: https://bsso.blpprofessional.com/as/device_authz.oauth2
  evidence:
  - body: '{"errors":[{"detail":"No definition of jwt found in header or query string."}]}'
    status: 401
    url: https://api.bloomberg.com/eap/
  - body: '{"error":"unauthorized_client","error_description":"No definition of jwt found in header or query string."}'
    status: 401
    url: https://api.bloomberg.com/eap/catalogs/
  - status: 200
    url: https://api.bloomberg.com/.well-known/oauth-protected-resource
  id: bloomberg_data_license_oauth2
  introspection_endpoint: https://bsso.blpprofessional.com/as/introspect.oauth2
  jwks_uri: https://bsso.blpprofessional.com/ext/caching/JWKS
  protected_resource: https://api.bloomberg.com
  protected_resource_metadata: https://api.bloomberg.com/.well-known/oauth-protected-resource
  registration_endpoint: https://bsso.blpprofessional.com/as/clients.oauth2
  revocation_endpoint: https://bsso.blpprofessional.com/as/revoke_token.oauth2
  token_endpoint: https://bsso.blpprofessional.com/as/token.oauth2
  token_format: JWT bearer
  transport: Authorization request header
  type: oauth2
- applies_to:
  - bloomberg.com account / entitlement identity (not the Data License data plane)
  authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize
  evidence:
  - status: 200
    url: https://www.bloomberg.com/.well-known/openid-configuration
  grant_types:
  - authorization_code
  - refresh_token
  id: bloomberg_com_oidc
  id_token_signing_alg: RS256
  issuer: https://www.bloomberg.com
  jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json
  openid_configuration: https://www.bloomberg.com/.well-known/openid-configuration
  pkce: S256
  token_endpoint: https://login.bloomberg.com/api/oauth/token
  type: openIdConnect
- applies_to:
  - Bloomberg B-PIPE API
  evidence:
  - status: 200
    url: https://bloomberg.github.io/blpapi-docs/
  id: blpapi_session_auth
  note: B-PIPE is not an HTTP API. It is consumed through the BLPAPI SDK over a TCP session (default port 8194) against a customer-provisioned B-PIPE appliance or a Bloomberg Server API host, with entitlement carried by the session identity (Terminal user or Application Name / EID) rather than by an HTTP credential. There is therefore no public HTTPS base URL and no bearer token for this entry.
  type: proprietary
slug: bloomberg-data-authentication
source_filename: bloomberg-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Bloomberg Data\nproviderId: bloomberg-data\ngenerated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://api.bloomberg.com/.well-known/oauth-protected-resource (200),\n  https://bsso.blpprofessional.com/.well-known/oauth-authorization-server (200),\n  https://www.bloomberg.com/.well-known/openid-configuration (200),\n  and live 401 challenges from https://api.bloomberg.com/eap/ and /eap/catalogs/\ndescription: >-\n  Authentication profile for the Bloomberg Data API surface. Derived from Bloomberg's own\n  published OAuth/OIDC discovery documents rather than from an OpenAPI document — Bloomberg\n  publishes no public machine-readable contract for the Data License REST API, but it does\n  publish RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata,\n  which name the token endpoint, the grant types and the flows exactly.\nschemes:\n  - id: bloomberg_data_license_oauth2\n\
  \    type: oauth2\n    applies_to:\n      - Bloomberg Data License API\n    protected_resource: https://api.bloomberg.com\n    protected_resource_metadata: https://api.bloomberg.com/.well-known/oauth-protected-resource\n    authorization_server: https://bsso.blpprofessional.com\n    authorization_server_metadata: https://bsso.blpprofessional.com/.well-known/oauth-authorization-server\n    token_endpoint: https://bsso.blpprofessional.com/as/token.oauth2\n    authorization_endpoint: https://bsso.blpprofessional.com/as/authorization.oauth2\n    introspection_endpoint: https://bsso.blpprofessional.com/as/introspect.oauth2\n    revocation_endpoint: https://bsso.blpprofessional.com/as/revoke_token.oauth2\n    device_authorization_endpoint: https://bsso.blpprofessional.com/as/device_authz.oauth2\n    registration_endpoint: https://bsso.blpprofessional.com/as/clients.oauth2\n    jwks_uri: https://bsso.blpprofessional.com/ext/caching/JWKS\n    token_format: JWT bearer\n    transport: Authorization\
  \ request header\n    credential_issuance: >-\n      Client credentials are issued to a contracted Data License customer from the Bloomberg\n      Enterprise Console (console.blpprofessional.com); there is no self-service signup.\n    evidence:\n      - url: https://api.bloomberg.com/eap/\n        status: 401\n        body: '{\"errors\":[{\"detail\":\"No definition of jwt found in header or query string.\"}]}'\n      - url: https://api.bloomberg.com/eap/catalogs/\n        status: 401\n        body: '{\"error\":\"unauthorized_client\",\"error_description\":\"No definition of jwt found in header or query string.\"}'\n      - url: https://api.bloomberg.com/.well-known/oauth-protected-resource\n        status: 200\n  - id: bloomberg_com_oidc\n    type: openIdConnect\n    applies_to:\n      - bloomberg.com account / entitlement identity (not the Data License data plane)\n    issuer: https://www.bloomberg.com\n    openid_configuration: https://www.bloomberg.com/.well-known/openid-configuration\n\
  \    authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize\n    token_endpoint: https://login.bloomberg.com/api/oauth/token\n    jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n    pkce: S256\n    id_token_signing_alg: RS256\n    evidence:\n      - url: https://www.bloomberg.com/.well-known/openid-configuration\n        status: 200\n  - id: blpapi_session_auth\n    type: proprietary\n    applies_to:\n      - Bloomberg B-PIPE API\n    note: >-\n      B-PIPE is not an HTTP API. It is consumed through the BLPAPI SDK over a TCP session\n      (default port 8194) against a customer-provisioned B-PIPE appliance or a Bloomberg\n      Server API host, with entitlement carried by the session identity (Terminal user or\n      Application Name / EID) rather than by an HTTP credential. There is therefore no\n      public HTTPS base URL and no bearer token for this entry.\n    evidence:\n \
  \     - url: https://bloomberg.github.io/blpapi-docs/\n        status: 200\nmtls: not-documented\napi_keys: false\nbasic_auth: false\ngaps:\n  - >-\n    The scope-to-operation mapping is not public. bsso.blpprofessional.com publishes\n    scopes_supported for identity (firmid, openid, profile, name, employeeid, bbprofile,\n    email) but the Data License data-plane entitlements are contract-provisioned, not\n    published as OAuth scopes.\n  - >-\n    No public auth quickstart page is reachable: www.bloomberg.com/professional/support/api-library/\n    returns a bot challenge (403) to non-browser clients and data.bloomberg.com renders\n    client-side behind a login.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-data/refs/heads/main/authentication/bloomberg-data-authentication.yml
summary_line: 3 schemes
tags:
- Analytics
- Financial-Services
- Market Data
- News
- Real-Time Data
- Trading
---
