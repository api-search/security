---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Upswing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upswing secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Upswing
provider_slug: upswing
scheme_count: 1
schemes:
- flow: authorizationCode
  identity_provider: https://idp.uat-upswing.one/realms/IntegrationDocs
  name: keycloak-oidc
  observed_at: https://integration-docs.upswing.one
  pkce: true
  scopes:
  - openid
  - profile
  - email
  sources:
  - live probe of integration-docs.upswing.one redirect
  type: openIdConnect
slug: upswing-authentication
source_filename: upswing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://integration-docs.upswing.one\nsummary:\n  types:\n  - openIdConnect\n  notes: >-\n    Upswing publishes no public OpenAPI, so no securitySchemes could be derived.\n    This profile is observed, not derived: the partner integration documentation\n    portal at https://integration-docs.upswing.one redirects unauthenticated\n    visitors to a Keycloak-hosted OpenID Connect authorization endpoint\n    (https://idp.uat-upswing.one/realms/IntegrationDocs/protocol/openid-connect/auth)\n    with PKCE (code_challenge) and scope \"openid profile email\". This confirms\n    the platform uses Keycloak / OpenID Connect for identity, but the underlying\n    partner API authentication model is not publicly documented and is governed\n    under commercial partner agreements.\nschemes:\n- name: keycloak-oidc\n  type: openIdConnect\n  observed_at: https://integration-docs.upswing.one\n  identity_provider: https://idp.uat-upswing.one/realms/IntegrationDocs\n\
  \  flow: authorizationCode\n  pkce: true\n  scopes:\n  - openid\n  - profile\n  - email\n  sources:\n  - live probe of integration-docs.upswing.one redirect\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upswing/refs/heads/main/authentication/upswing-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Fintech
- Open Finance
- Embedded Finance
- Banking
- India
- Deposits
- Lending
---
