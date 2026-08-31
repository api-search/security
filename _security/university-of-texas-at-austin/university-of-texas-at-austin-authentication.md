---
api_key_in: []
api_specs:
- filename: university-of-texas-at-austin-tapis-systems-openapi.yml
  format: yaml
  label: Tapis v3 Research Computing Platform (TACC production tenant)
  slug: tapis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-texas-at-austin/refs/heads/main/openapi/university-of-texas-at-austin-tapis-systems-openapi.yml
auth_types: []
description: How each University of Texas at Austin surface authenticates. Every entry was observed on a live unauthenticated request; nothing here is inferred from documentation prose.
kind: authentication
layout: security
method: probed
name: University Of Texas At Austin Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Texas at Austin declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Texas at Austin
provider_slug: university-of-texas-at-austin
scheme_count: 0
schemes: []
slug: university-of-texas-at-austin-authentication
source_filename: university-of-texas-at-austin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Texas at Austin — authentication\ndescription: >-\n  How each University of Texas at Austin surface authenticates. Every entry was\n  observed on a live unauthenticated request; nothing here is inferred from\n  documentation prose.\ngenerated: '2026-08-30'\nmethod: probed\nsource: live HTTP probes 2026-08-30 (see examples/)\nmechanisms:\n  - surface: UT Austin Enterprise Identity Provider\n    x-operator: institution\n    software: Shibboleth Identity Provider\n    protocols:\n      - name: SAML 2.0 Web SSO\n        entity_id: https://enterprise.login.utexas.edu/idp/shibboleth\n        metadata_url: https://enterprise.login.utexas.edu/idp/shibboleth\n        status: 200\n        bindings:\n          - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n          - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          - urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n        federation:\
  \ InCommon\n        federation_metadata_url: https://mdq.incommon.org/entities/https%3A%2F%2Fenterprise.login.utexas.edu%2Fidp%2Fshibboleth\n        federation_status: 200\n        generated: '2026-08-30'\n        method: probed\n        source: https://enterprise.login.utexas.edu/idp/shibboleth\n      - name: OpenID Connect 1.0\n        issuer: https://enterprise.login.utexas.edu\n        discovery_url: https://enterprise.login.utexas.edu/.well-known/openid-configuration\n        status: 200\n        authorization_endpoint: https://enterprise.login.utexas.edu/idp/profile/oidc/authorize\n        token_endpoint: https://enterprise.login.utexas.edu/idp/profile/oidc/token\n        userinfo_endpoint: https://enterprise.login.utexas.edu/idp/profile/oidc/userinfo\n        jwks_uri: https://enterprise.login.utexas.edu/idp/profile/oidc/keyset\n        introspection_endpoint: https://enterprise.login.utexas.edu/idp/profile/oauth2/introspection\n        revocation_endpoint: https://enterprise.login.utexas.edu/idp/profile/oauth2/revocation\n\
  \        end_session_endpoint: https://enterprise.login.utexas.edu/idp/profile/oidc/end-session\n        registration_endpoint: https://enterprise.login.utexas.edu/idp/profile/oidc/register\n        dynamic_client_registration: true\n        grant_types_supported: [ authorization_code, refresh_token ]\n        token_endpoint_auth_methods_supported:\n          - client_secret_basic\n          - client_secret_post\n          - client_secret_jwt\n          - private_key_jwt\n        subject_types_supported: [ public, pairwise ]\n        generated: '2026-08-30'\n        method: probed\n        source: https://enterprise.login.utexas.edu/.well-known/openid-configuration\n    note: >-\n      Client registration is not self-service. The registration_endpoint is\n      advertised in the discovery document but issuing credentials is an\n      institutional process run through UT Austin Identity and Access\n      Management; no public developer sign-up was found.\n  - surface: Texas ScholarWorks\
  \ DSpace REST API\n    x-operator: institution\n    base_url: https://repositories.lib.utexas.edu/server/api\n    anonymous_read: true\n    anonymous_read_status: 200\n    challenge_header: >-\n      shibboleth realm=\"DSpace REST API\",\n      location=\"https://repositories.lib.utexas.edu/Shibboleth.sso/Login?target=https%3A%2F%2Frepositories.lib.utexas.edu%2Fserver%2Fapi%2Fauthn%2Fshibboleth\",\n      password realm=\"DSpace REST API\"\n    schemes:\n      - name: Shibboleth SSO\n        detail: >-\n          Advertised in the WWW-Authenticate header on\n          /server/api/authn/status. Routes to the institution's own\n          Shibboleth.sso service provider.\n      - name: Password (EPerson)\n        detail: DSpace native login against a repository account.\n    csrf: DSpace requires an X-XSRF-TOKEN header for state-changing requests.\n    generated: '2026-08-30'\n    method: probed\n    source: https://repositories.lib.utexas.edu/server/api/authn/status\n  - surface: Tapis v3\
  \ platform — TACC production tenant\n    x-operator: institution\n    base_url: https://tacc.tapis.io/v3\n    anonymous_read: false\n    scheme: JWT bearer token (X-Tapis-Token header), issued by the tenant authenticator\n    authenticator: https://tacc.tapis.io/v3/oauth2\n    observed_rejection: >-\n      HTTP 401 \"TAPIS_SECURITY_MISSING_JWT_INFO HTTP GET request rejected due to\n      missing JSON Web Token information.\" on GET /v3/systems\n    account_prerequisite: A TACC user account; allocation required for compute resources.\n    generated: '2026-08-30'\n    method: probed\n    source: https://tacc.tapis.io/v3/systems\n  - surface: Texas Data Repository (Dataverse)\n    x-operator: tenant\n    base_url: https://dataverse.tdl.org/api\n    anonymous_read: true\n    anonymous_read_status: 200\n    scheme: X-Dataverse-key API token for write operations\n    note: >-\n      The authentication model is the Texas Digital Library's, not UT Austin's.\n      Recorded because UT Austin's\
  \ research data lands here, not because UT\n      Austin operates it.\n    generated: '2026-08-30'\n    method: probed\n    source: https://dataverse.tdl.org/api/dataverses/utexas\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-texas-at-austin/refs/heads/main/authentication/university-of-texas-at-austin-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Texas
- Research Computing
- Identity Federation
- Institutional Repository
- Research Data
- Library
- Open Data
---
