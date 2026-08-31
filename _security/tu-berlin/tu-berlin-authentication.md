---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tu Berlin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Technical University of Berlin declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: Technical University of Berlin
provider_slug: tu-berlin
scheme_count: 7
schemes:
- description: The institution's Shibboleth Identity Provider. Its SAML 2.0 metadata is public and machine-readable (200, application/xml, 15,920 bytes) and carries both an IDPSSODescriptor and an AttributeAuthorityDescriptor. This is the one API-shaped surface a university operates by definition, and it is TU Berlin's own.
  docs: https://www.tu.berlin/campusmanagement/angebot/shibboleth
  endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/SAML2/Redirect/SSO
    service: SingleSignOnService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/SAML2/POST/SSO
    service: SingleSignOnService
  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest
    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/Shibboleth/SSO
    service: SingleSignOnService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/SAML2/Redirect/SLO
    service: SingleLogoutService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
    location: https://shibboleth.tubit.tu-berlin.de:8443/idp/profile/SAML2/SOAP/AttributeQuery
    service: AttributeService
  entity_id: https://ephraim.tu-berlin.de/shibboleth
  federation: DFN-AAI (German National Research and Education Network federation)
  metadata_url: https://shibboleth.tu-berlin.de/idp/shibboleth
  name: shibboleth-saml2-idp
  operator: institution
  scope: tu-berlin.de
  sources:
  - https://shibboleth.tu-berlin.de/idp/shibboleth
  type: saml2
- description: The self-hosted GitLab instance is its own OAuth 2.0 authorization server and OIDC provider. Human login is brokered to Shibboleth SSO; the OAuth endpoints are the programmatic path. Scopes are listed in scopes/tu-berlin-scopes.yml.
  discovery: https://git.tu-berlin.de/.well-known/openid-configuration
  flows:
  - authorizationUrl: https://git.tu-berlin.de/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://git.tu-berlin.de/oauth/token
  - flow: clientCredentials
    tokenUrl: https://git.tu-berlin.de/oauth/token
  - flow: deviceCode
    tokenUrl: https://git.tu-berlin.de/oauth/token
  introspection_endpoint: https://git.tu-berlin.de/oauth/introspect
  issuer: https://git.tu-berlin.de
  jwks_uri: https://git.tu-berlin.de/oauth/discovery/keys
  name: gitlab-oauth2-oidc
  operator: institution
  revocation_endpoint: https://git.tu-berlin.de/oauth/revoke
  sources:
  - well-known/tu-berlin-gitlab-openid-configuration.json
  type: oauth2
  userinfo_endpoint: https://git.tu-berlin.de/oauth/userinfo
- description: GitLab REST v4 accepts PRIVATE-TOKEN / Bearer credentials. Read access to PUBLIC projects needs no credential at all — https://git.tu-berlin.de/api/v4/projects returns 200 with X-Total 2851 unauthenticated — while /api/v4/version and /api/v4/metadata return 401.
  in: header
  name: gitlab-personal-access-token
  operator: institution
  scheme: bearer
  sources:
  - https://git.tu-berlin.de/api/v4/projects?visibility=public
  type: http
- auth_url: https://isis.tu-berlin.de/mod/lti/auth.php
  description: 'ISIS (the TU Berlin Moodle) acts as an LTI 1.3 platform: a public RS256 JWKS is served for tool integrations, with the standard OIDC-launch auth endpoint and a client-credentials token endpoint. This is the institution''s learning-tool interoperability surface.'
  keyset_url: https://isis.tu-berlin.de/mod/lti/certs.php
  name: moodle-lti-1p3-platform
  operator: institution
  sources:
  - https://isis.tu-berlin.de/mod/lti/certs.php
  token_url: https://isis.tu-berlin.de/mod/lti/token.php
  type: oauth2
- description: 'The Moodle web-service endpoint is enabled but closed: GET https://isis.tu-berlin.de/webservice/rest/server.php returns 200 with an XML moodle_exception, ERRORCODE invalidtoken. Tokens are issued to TU Berlin accounts only; there is no public self-service path.'
  in: query
  name: moodle-webservice-token
  operator: institution
  parameter: wstoken
  sources:
  - https://isis.tu-berlin.de/webservice/rest/server.php
  type: apiKey
- description: 'The DepositOnce DSpace 9 REST API exposes /server/api/authn for login and a JWT-bearer session. Anonymous read is genuinely partial: /server/api and /server/api/discover/search/objects return 200 unauthenticated, while /server/api/core/items returns 401. OAI-PMH is fully open.'
  name: dspace-authn
  operator: institution
  scheme: bearer
  sources:
  - https://api-depositonce.tu-berlin.de/server/api
  - https://api-depositonce.tu-berlin.de/server/api/core/items?size=1
  type: http
- description: The TU Berlin Synapse homeserver advertises its login flows unauthenticated — https://matrix.tu-berlin.de/_matrix/client/v3/login returns 200 with m.login.password and m.login.application_service. Guest access is disabled in the published Element config; authenticated calls carry a Matrix access token.
  name: matrix-login
  operator: institution
  scheme: bearer
  sources:
  - https://matrix.tu-berlin.de/_matrix/client/v3/login
  type: http
slug: tu-berlin-authentication
source_filename: tu-berlin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live unauthenticated probes on 2026-08-30 of shibboleth.tu-berlin.de,\n  git.tu-berlin.de, isis.tu-berlin.de, api-depositonce.tu-berlin.de and\n  matrix.tu-berlin.de.\nnote: >-\n  TU Berlin publishes no OpenAPI, so nothing here is derived from a contract. Each scheme\n  below was read from a live machine-readable document served on a host under a TU Berlin\n  registrable domain. Institutional login across services is Shibboleth/SAML via DFN-AAI,\n  operated by the ZECM; individual services layer their own product authentication on top\n  of it.\n  This file was generated by API Evangelist from live probes on 2026-08-30; TU Berlin did\n  not publish it. Only well-known/tu-berlin-gitlab-openid-configuration.json is TU Berlin's\n  own document, fetched verbatim from its GitLab instance.\nschemes:\n- name: shibboleth-saml2-idp\n  type: saml2\n  operator: institution\n  entity_id: https://ephraim.tu-berlin.de/shibboleth\n  metadata_url:\
  \ https://shibboleth.tu-berlin.de/idp/shibboleth\n  federation: DFN-AAI (German National Research and Education Network federation)\n  scope: tu-berlin.de\n  endpoints:\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    service: SingleSignOnService\n    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/SAML2/Redirect/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    service: SingleSignOnService\n    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/SAML2/POST/SSO\n  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n    service: SingleSignOnService\n    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/Shibboleth/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    service: SingleLogoutService\n    location: https://shibboleth.tubit.tu-berlin.de/idp/profile/SAML2/Redirect/SLO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    service: AttributeService\n    location: https://shibboleth.tubit.tu-berlin.de:8443/idp/profile/SAML2/SOAP/AttributeQuery\n\
  \  description: >-\n    The institution's Shibboleth Identity Provider. Its SAML 2.0 metadata is public and\n    machine-readable (200, application/xml, 15,920 bytes) and carries both an\n    IDPSSODescriptor and an AttributeAuthorityDescriptor. This is the one API-shaped\n    surface a university operates by definition, and it is TU Berlin's own.\n  docs: https://www.tu.berlin/campusmanagement/angebot/shibboleth\n  sources:\n  - https://shibboleth.tu-berlin.de/idp/shibboleth\n- name: gitlab-oauth2-oidc\n  type: oauth2\n  operator: institution\n  issuer: https://git.tu-berlin.de\n  discovery: https://git.tu-berlin.de/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://git.tu-berlin.de/oauth/authorize\n    tokenUrl: https://git.tu-berlin.de/oauth/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://git.tu-berlin.de/oauth/token\n  - flow: deviceCode\n    tokenUrl: https://git.tu-berlin.de/oauth/token\n  jwks_uri: https://git.tu-berlin.de/oauth/discovery/keys\n\
  \  userinfo_endpoint: https://git.tu-berlin.de/oauth/userinfo\n  introspection_endpoint: https://git.tu-berlin.de/oauth/introspect\n  revocation_endpoint: https://git.tu-berlin.de/oauth/revoke\n  description: >-\n    The self-hosted GitLab instance is its own OAuth 2.0 authorization server and OIDC\n    provider. Human login is brokered to Shibboleth SSO; the OAuth endpoints are the\n    programmatic path. Scopes are listed in scopes/tu-berlin-scopes.yml.\n  sources:\n  - well-known/tu-berlin-gitlab-openid-configuration.json\n- name: gitlab-personal-access-token\n  type: http\n  scheme: bearer\n  operator: institution\n  in: header\n  description: >-\n    GitLab REST v4 accepts PRIVATE-TOKEN / Bearer credentials. Read access to PUBLIC\n    projects needs no credential at all — https://git.tu-berlin.de/api/v4/projects\n    returns 200 with X-Total 2851 unauthenticated — while /api/v4/version and\n    /api/v4/metadata return 401.\n  sources:\n  - https://git.tu-berlin.de/api/v4/projects?visibility=public\n\
  - name: moodle-lti-1p3-platform\n  type: oauth2\n  operator: institution\n  keyset_url: https://isis.tu-berlin.de/mod/lti/certs.php\n  token_url: https://isis.tu-berlin.de/mod/lti/token.php\n  auth_url: https://isis.tu-berlin.de/mod/lti/auth.php\n  description: >-\n    ISIS (the TU Berlin Moodle) acts as an LTI 1.3 platform: a public RS256 JWKS is served\n    for tool integrations, with the standard OIDC-launch auth endpoint and a\n    client-credentials token endpoint. This is the institution's learning-tool\n    interoperability surface.\n  sources:\n  - https://isis.tu-berlin.de/mod/lti/certs.php\n- name: moodle-webservice-token\n  type: apiKey\n  operator: institution\n  in: query\n  parameter: wstoken\n  description: >-\n    The Moodle web-service endpoint is enabled but closed: GET\n    https://isis.tu-berlin.de/webservice/rest/server.php returns 200 with an XML\n    moodle_exception, ERRORCODE invalidtoken. Tokens are issued to TU Berlin accounts\n    only; there is no public self-service\
  \ path.\n  sources:\n  - https://isis.tu-berlin.de/webservice/rest/server.php\n- name: dspace-authn\n  type: http\n  scheme: bearer\n  operator: institution\n  description: >-\n    The DepositOnce DSpace 9 REST API exposes /server/api/authn for login and a JWT-bearer\n    session. Anonymous read is genuinely partial: /server/api and\n    /server/api/discover/search/objects return 200 unauthenticated, while\n    /server/api/core/items returns 401. OAI-PMH is fully open.\n  sources:\n  - https://api-depositonce.tu-berlin.de/server/api\n  - https://api-depositonce.tu-berlin.de/server/api/core/items?size=1\n- name: matrix-login\n  type: http\n  scheme: bearer\n  operator: institution\n  description: >-\n    The TU Berlin Synapse homeserver advertises its login flows unauthenticated —\n    https://matrix.tu-berlin.de/_matrix/client/v3/login returns 200 with\n    m.login.password and m.login.application_service. Guest access is disabled in the\n    published Element config; authenticated calls\
  \ carry a Matrix access token.\n  sources:\n  - https://matrix.tu-berlin.de/_matrix/client/v3/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-berlin/refs/heads/main/authentication/tu-berlin-authentication.yml
summary_line: 7 schemes
tags:
- University
- Higher Education
- Education
- Technical University
- Germany
- Berlin
- Research Data
- Open Access
- Repository
- Library
- Identity Federation
- Course Catalog
- Research Computing
---
