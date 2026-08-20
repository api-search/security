---
api_key_in: []
api_specs:
- filename: tum-campus-backend-openapi.yml
  format: yaml
  label: TUM Campus App Backend API
  slug: campus-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-campus-backend-openapi.yml
- filename: tum-locations-api-openapi.yml
  format: yaml
  label: NavigaTUM
  slug: navigatum
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-locations-api-openapi.yml
- filename: tum-menu-api-openapi.yml
  format: yaml
  label: eat-api — Munich Student Canteen Menus
  slug: eat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-menu-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Technical University of Munich declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Technical University of Munich
provider_slug: tum
scheme_count: 0
schemes: []
slug: tum-authentication
source_filename: tum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of every surface attributed to Technical University of Munich, plus\n  the security schemes declared in the contracts saved under openapi/. Each entry carries the\n  operator of the thing it describes — an institution's authentication story is mostly its\n  vendors' authentication stories, and this artifact refuses to blur the two.\nsurfaces:\n\n- surface: TUM Campus App Backend API\n  x-operator: institution\n  base_url: https://api.tum.app/v1\n  scheme: none\n  detail: >-\n    The generated contract declares no securityDefinitions and no global security requirement, and\n    the read operations answer unauthenticated (GET /v1/news/sources 200, GET /v1/student_clubs 200,\n    GET /v1/dish/rating/allDishTags 200). Write operations (POST /v1/device, POST /v1/feedback,\n    POST /v1/*/rating/new) are governed by a device registration and an in-band token carried in the\n    request body rather than\
  \ by a declared security scheme, so no scheme is discoverable from the\n    contract. This is a real contract gap, not a finding of \"open write access\".\n  evidence:\n  - url: https://api.tum.app/v1/news/sources\n    status: 200\n  - url: https://api.tum.app/swagger/swagger.json\n    status: 200\n\n- surface: NavigaTUM\n  x-operator: institution\n  base_url: https://nav.tum.de/api\n  scheme: none\n  detail: >-\n    Fully unauthenticated read API. Search, location lookup, maps and calendar answer without\n    credentials. The feedback endpoints use a short-lived token issued by GET /api/feedback/get_token\n    as an anti-abuse measure; it is not an identity credential and grants no user context.\n  evidence:\n  - url: https://nav.tum.de/api/search?q=mi\n    status: 200\n  - url: https://nav.tum.de/api/status\n    status: 200\n\n- surface: eat-api\n  x-operator: tenant\n  base_url: https://tum-dev.github.io/eat-api\n  scheme: none\n  detail: >-\n    Static JSON files on GitHub Pages. No\
  \ authentication exists or could exist.\n  evidence:\n  - url: https://tum-dev.github.io/eat-api/enums/canteens.json\n    status: 200\n\n- surface: TUMonline (CAMPUSonline)\n  x-operator: tenant\n  base_url: https://campus.tum.de/tumonline\n  scheme: oauth2\n  openid_configuration: >-\n    https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/.well-known/openid-configuration\n  detail: >-\n    TUM's student information system runs CAMPUSonline, and its Keycloak realm publishes a complete\n    OpenID Connect discovery document on TUM's own campus.tum.de host. The realm is named\n    CAMPUSonline, not TUM — the contract shape is the vendor's; the deployment, the users and the\n    data are TUM's. This is the operator distinction this pipeline exists to keep straight, so it is\n    recorded as a tenant relationship and NOT saved as a TUM contract.\n  endpoints:\n    issuer: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline\n    authorization: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/protocol/openid-connect/auth\n\
  \    token: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/protocol/openid-connect/token\n    userinfo: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/protocol/openid-connect/userinfo\n    jwks: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/protocol/openid-connect/certs\n    introspection: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/protocol/openid-connect/token/introspect\n    end_session: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/protocol/openid-connect/logout\n    dynamic_registration: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/clients-registrations/openid-connect\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n\
  \  pkce_methods:\n  - plain\n  - S256\n  notes:\n  - >-\n    The realm still advertises the implicit and resource-owner-password grants alongside\n    authorization_code + PKCE. Both are discouraged by OAuth 2.1 / BCP 225.\n  evidence:\n  - url: https://campus.tum.de/tumonline/co/public/sec/auth/realms/CAMPUSonline/.well-known/openid-configuration\n    status: 200\n\n- surface: TUM Shibboleth Identity Provider\n  x-operator: institution\n  base_url: https://login.tum.de/idp\n  scheme: saml2\n  detail: >-\n    SAML 2.0 / Shibboleth IdP, DFN-AAI registered, eduGAIN reachable, asserting scope tum.de and\n    carrying REFEDS Research & Scholarship plus SIRTFI and SIRTFI2 assurance certifications. This is\n    the one authentication surface a university operates by definition, and it is machine-readable.\n  evidence:\n  - url: https://login.tum.de/idp/shibboleth\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/authentication/tum-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Germany
- Technical University
- Universities of Excellence
- Campus
- Course Catalog
- Identity Federation
- Research Repository
- Open-Source
- Student Information System
---
