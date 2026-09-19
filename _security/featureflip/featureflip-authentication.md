---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: featureflip-client-sdk-api-openapi.yml
  format: yaml
  label: Featureflip Client SDK API
  slug: featureflip-client-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-client-sdk-api-openapi.yml
- filename: featureflip-environments-api-openapi.yml
  format: yaml
  label: Featureflip Environments API
  slug: featureflip-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-environments-api-openapi.yml
- filename: featureflip-feature-flags-api-openapi.yml
  format: yaml
  label: Featureflip Feature Flags API
  slug: featureflip-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-feature-flags-api-openapi.yml
- filename: featureflip-me-api-openapi.yml
  format: yaml
  label: Featureflip Me API
  slug: featureflip-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-me-api-openapi.yml
- filename: featureflip-organizations-api-openapi.yml
  format: yaml
  label: Featureflip Organizations API
  slug: featureflip-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-organizations-api-openapi.yml
- filename: featureflip-projects-api-openapi.yml
  format: yaml
  label: Featureflip Projects API
  slug: featureflip-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-projects-api-openapi.yml
- filename: featureflip-sdk-keys-api-openapi.yml
  format: yaml
  label: Featureflip SDK Keys API
  slug: featureflip-sdk-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-sdk-keys-api-openapi.yml
- filename: featureflip-server-sdk-api-openapi.yml
  format: yaml
  label: Featureflip Server SDK API
  slug: featureflip-server-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-server-sdk-api-openapi.yml
- filename: featureflip-user-segments-api-openapi.yml
  format: yaml
  label: Featureflip User Segments API
  slug: featureflip-user-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-user-segments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Featureflip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Featureflip secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Featureflip
provider_slug: featureflip
scheme_count: 1
schemes:
- format: Bearer <token>
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/featureflip-evaluation-api.json
  - openapi/featureflip-management-api.json
  type: apiKey
slug: featureflip-authentication
source_filename: featureflip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://featureflip.io/docs/management-api/authentication/ enriched over the\n  securityScheme derived from openapi/featureflip-management-api.json and\n  openapi/featureflip-evaluation-api.json.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  note: Bearer token in the Authorization header; no OAuth2/OIDC.\nschemes:\n  - name: Bearer\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: \"Bearer <token>\"\n    sources:\n      - openapi/featureflip-evaluation-api.json\n      - openapi/featureflip-management-api.json\nmanagement_api:\n  token_types:\n    - prefix: ffp_\n      name: Personal Access Token\n      identity: Individual user across all organizations they belong to\n      created_in: Settings -> API Tokens -> Personal Access Tokens\n    - prefix: ffs_\n      name: Service Token\n      identity: Machine identity scoped to a single organization with an explicit\
  \ role\n      created_in: Organization Settings -> Service Tokens\n      features: [project allowlist, optional expiry, immediate revocation]\n  roles:\n    - Owner    # full access incl. org settings\n    - Admin    # project, flag, and member management\n    - Member   # flag create/edit, targeting, segments\n    - Viewer   # read-only\n  failure:\n    insufficient_role: 403 forbidden\n    excluded_project: 404 not_found  # service token project allowlist\n    missing_malformed_expired_revoked: 401 unauthorized\nevaluation_api:\n  auth: 'SDK key sent as \"Authorization: Bearer <sdk-key>\"'\n  scope: Per-environment. A client SDK key returns only client-side-visible flags as pre-evaluated values; a server SDK key sees every flag in the project.\naccount_security:\n  two_factor: TOTP authenticator app + recovery codes (all plans)\n  sso: Sign in with Google (all plans); SAML/SCIM on Enterprise\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/authentication/featureflip-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Feature Flags
- Feature Management
- feature flag cleanup
- Progressive Delivery
- Experimentation
- feature flags as code
- OpenFeature
- MCP
- Developer Tools
- DevOps/CI-CD
---
