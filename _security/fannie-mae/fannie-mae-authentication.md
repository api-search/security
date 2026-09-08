---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Fannie Mae Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fannie Mae declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Fannie Mae
provider_slug: fannie-mae
scheme_count: 4
schemes:
- description: The Developer Portal front door. An unauthenticated request to the portal's own data API 302s to fmsso.fanniemae.com/as/authorization.oauth2 with client_id=sso-p2p-GED-p1-oidc-iDMZ-DeveloperPortal, response_type=code and scope="openid profile idmz".
  evidence: HTTP 302 observed 2026-09-07 on https://developer.fanniemae.com/fv7ui-secured/web/fv7/api/auth/v1/userdetails
  flow: authorizationCode
  id: oauth2_authorization_code
  pkce: supported (S256)
  type: oauth2
- description: Advertised in grant_types_supported. This is the machine-to-machine path a licensed integrator would use for API calls; issuance of a client is not self-service.
  evidence: https://fmsso.fanniemae.com/.well-known/oauth-authorization-server
  flow: clientCredentials
  id: oauth2_client_credentials
  type: oauth2
- description: tls_client_auth is advertised as a token-endpoint client authentication method.
  evidence: https://fmsso.fanniemae.com/.well-known/oauth-authorization-server
  id: mutual_tls
  type: mutualTLS
- description: SAML 2.0 bearer grant and PingFederate IdP-initiated SSO/SLO (https://fmsso.fanniemae.com/idp/startSLO.ping) — the enterprise federation path used by licensed seller/servicer organizations.
  evidence: https://fmsso.fanniemae.com/.well-known/openid-configuration
  id: saml2_federation
  type: saml
slug: fannie-mae-authentication
source_filename: fannie-mae-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  https://fmsso.fanniemae.com/.well-known/openid-configuration (HTTP 200, application/json, fetched\n  2026-09-07) and https://fmsso.fanniemae.com/.well-known/oauth-authorization-server (HTTP 200), both\n  saved verbatim under well-known/. Reached by following the Developer Portal's own 302 from\n  https://developer.fanniemae.com/fv7ui-secured/web/fv7/api/auth/v1/userdetails.\nnote: >-\n  Derived from Fannie Mae's own published authorization-server metadata, not from an OpenAPI —\n  Fannie Mae publishes no public API contract. This describes how a developer authenticates to the\n  Fannie Mae Developer Portal and to the applications and APIs behind it; per-API security schemes\n  are not public.\nprovider: Fannie Mae\nauthorization_servers:\n  - issuer: https://fmsso.fanniemae.com\n    product: PingFederate\n    role: primary — external party / Developer Portal SSO\n    discovery:\n      openid_configuration: https://fmsso.fanniemae.com/.well-known/openid-configuration\n\
  \      oauth_authorization_server: https://fmsso.fanniemae.com/.well-known/oauth-authorization-server\n      jwks_uri: https://fmsso.fanniemae.com/pf/JWKS\n    endpoints:\n      authorization: https://fmsso.fanniemae.com/as/authorization.oauth2\n      token: https://fmsso.fanniemae.com/as/token.oauth2\n      userinfo: https://fmsso.fanniemae.com/idp/userinfo.openid\n      introspection: https://fmsso.fanniemae.com/as/introspect.oauth2\n      revocation: https://fmsso.fanniemae.com/as/revoke_token.oauth2\n      end_session: https://fmsso.fanniemae.com/idp/init_logout.openid\n      pushed_authorization_request: https://fmsso.fanniemae.com/as/par.oauth2\n      device_authorization: https://fmsso.fanniemae.com/as/device_authz.oauth2\n      backchannel_authentication: https://fmsso.fanniemae.com/as/bc-auth.ciba\n      dynamic_client_registration: https://fmsso.fanniemae.com/as/clients.oauth2\n    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n \
  \     - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:saml2-bearer\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:openid:params:grant-type:ciba\n      - urn:pingidentity.com:oauth2:grant_type:validate_bearer\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - tls_client_auth\n      - none\n    code_challenge_methods_supported: [plain, S256]\n    require_pushed_authorization_requests: false\n    subject_types_supported: [public, pairwise]\n    claims_supported: [sub]\n    dpop_supported: true\n    mtls_client_auth_supported: true\n  - issuer: https://auth.pingone.com/4c2b23f9-52b1-4f8f-aa1f-1d477590770c/as\n    product: PingOne (Fannie Mae production tenant)\n    role: >-\n      Developer Portal self-service registration.\
  \ The production portal's shipped runtime config\n      names this environment as its registerUrl; the environment id was read from\n      https://developer.fanniemae.com/main.9ce4eb977e10f81d.js.\n    discovery:\n      openid_configuration: https://auth.pingone.com/4c2b23f9-52b1-4f8f-aa1f-1d477590770c/as/.well-known/openid-configuration\n    probed_status: 200\n    note: >-\n      Served by Ping Identity's SaaS on a Fannie Mae tenant, not on a fanniemae.com host — recorded as\n      evidence, not counted as a document Fannie Mae serves.\nschemes:\n  - id: oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n    pkce: supported (S256)\n    description: >-\n      The Developer Portal front door. An unauthenticated request to the portal's own data API\n      302s to fmsso.fanniemae.com/as/authorization.oauth2 with\n      client_id=sso-p2p-GED-p1-oidc-iDMZ-DeveloperPortal, response_type=code and\n      scope=\"openid profile idmz\".\n    evidence: >-\n      HTTP 302 observed\
  \ 2026-09-07 on\n      https://developer.fanniemae.com/fv7ui-secured/web/fv7/api/auth/v1/userdetails\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Advertised in grant_types_supported. This is the machine-to-machine path a licensed integrator\n      would use for API calls; issuance of a client is not self-service.\n    evidence: https://fmsso.fanniemae.com/.well-known/oauth-authorization-server\n  - id: mutual_tls\n    type: mutualTLS\n    description: tls_client_auth is advertised as a token-endpoint client authentication method.\n    evidence: https://fmsso.fanniemae.com/.well-known/oauth-authorization-server\n  - id: saml2_federation\n    type: saml\n    description: >-\n      SAML 2.0 bearer grant and PingFederate IdP-initiated SSO/SLO\n      (https://fmsso.fanniemae.com/idp/startSLO.ping) — the enterprise federation path used by\n      licensed seller/servicer organizations.\n    evidence: https://fmsso.fanniemae.com/.well-known/openid-configuration\n\
  access:\n  self_service_registration: true\n  registration_url: https://auth.pingone.com/4c2b23f9-52b1-4f8f-aa1f-1d477590770c/saml20/idp/startsso?spEntityId=p1c-puma-GED-p1-saml-devportal-DirectRegistration\n  registration_probed_status: 200\n  credentials_gate: >-\n    A free Developer Portal account can be self-registered, but production API access is granted per\n    application under the Software Subscription Agreement (the Consolidated Technology Guide) and is\n    administered through Technology Manager — it is not self-service.\n  contract_published: false\n  api_reference_public: false\ndocs:\n  developer_portal: https://developer.fanniemae.com/\n  get_started: https://developer.fanniemae.com/#/get-started\n  technology_guide: https://www.fanniemae.com/tech-guide\n  technology_manager: https://technologymanager.fanniemae.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fannie-mae/refs/heads/main/authentication/fannie-mae-authentication.yml
summary_line: 4 schemes
tags:
- Federal-Government
- Housing
- Mortgages
- Finance
- GSE
- Fortune 100
---
