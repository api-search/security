---
anonymous_access: false
api_key_in: []
api_specs:
- filename: facets-control-plane-openapi.yml
  format: yaml
  label: Facets Control Plane API
  slug: facets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facets/refs/heads/main/openapi/facets-control-plane-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Facets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facets secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Facets
provider_slug: facets
scheme_count: 1
schemes:
- applies_to: document-level `security` - every operation except the /public/v1 surface
  credentials:
    docs: https://www.facets.cloud/docs/api/recipes/authentication-setup
    password: A personal access token generated inside the Control Plane, NOT your login password. Account Settings -> Personal Token -> Generate Token. The token string is displayed once in the creation pop-up and cannot be retrieved afterwards.
    token_page: <control-plane-url>/v2/home#personal-access-tokens
    username: The email address you sign in to the Facets Control Plane with.
  description: Basic Authentication
  machine_credentials:
    credentials_file: ~/.facets/credentials
    env_vars:
    - FACETS_USERNAME
    - FACETS_TOKEN
    - CONTROL_PLANE_URL
    note: The same three environment variables authenticate raptor in CI, all three MCP servers, and praxis. A `raptor login` writes the profile that every other Facets tool reads.
    profile_env: FACETS_PROFILE
    service_account: Release v0.94 added a built-in ci-user service account for automation; the spec carries a Service Accounts tag with 4 operations.
  name: basicAuth
  rotation:
    documented: false
    expiry: not documented
    revocation: Tokens are listed and managed on the Personal Token page; no API operation for rotation is documented.
  scheme: basic
  sources:
  - openapi/facets-control-plane-openapi.yml
  type: http
slug: facets-authentication
source_filename: facets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: openapi/facets-control-plane-openapi.yml\ndocs: https://www.facets.cloud/docs/api/recipes/authentication-setup\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic Authentication\n  sources:\n  - openapi/facets-control-plane-openapi.yml\n  applies_to: document-level `security` - every operation except the /public/v1 surface\n  credentials:\n    username: The email address you sign in to the Facets Control Plane with.\n    password: >-\n      A personal access token generated inside the Control Plane, NOT your login password.\n      Account Settings -> Personal Token -> Generate Token. The token string is displayed\n      once in the creation pop-up and cannot be retrieved afterwards.\n    token_page: <control-plane-url>/v2/home#personal-access-tokens\n    docs: https://www.facets.cloud/docs/api/recipes/authentication-setup\n\
  \  machine_credentials:\n    env_vars: [FACETS_USERNAME, FACETS_TOKEN, CONTROL_PLANE_URL]\n    credentials_file: ~/.facets/credentials\n    profile_env: FACETS_PROFILE\n    note: >-\n      The same three environment variables authenticate raptor in CI, all three MCP servers,\n      and praxis. A `raptor login` writes the profile that every other Facets tool reads.\n    service_account: 'Release v0.94 added a built-in ci-user service account for automation; the spec carries a Service Accounts tag with 4 operations.'\n  rotation:\n    documented: false\n    expiry: not documented\n    revocation: 'Tokens are listed and managed on the Personal Token page; no API operation for rotation is documented.'\nunauthenticated_surface:\n  note: The /public/v1 operations answer without credentials and describe the control plane before login.\n  operations: [healthCheck, getLoginOptions, getSamlLoginOptions, getAllFeatureProperties, getFeatureProperty, getCPCloud, getModuleSchema, getModuleSchemaByType,\
  \ getLogo, retrieveThemeFile]\nconsole_sso:\n  note: >-\n    DISTINCT FROM API AUTH - included because it is easy to conflate. Human sign-in to the\n    Facets console supports OAuth and SAML SSO (Google, Okta, Azure AD, OneLogin, JumpCloud,\n    generic SSO). None of it applies to the API, which is HTTP Basic only.\n  docs: https://www.facets.cloud/docs/features-and-guides/authentication-and-sso\nauthorization:\n  model: RBAC\n  docs: https://www.facets.cloud/docs/features-and-guides/rbac\n  features: [users, user groups, user roles, custom roles, custom Kubernetes roles, resource groups]\n  ai_permissions:\n    note: >-\n      Roles carry a separate AI Permissions setting. By default AI actions inherit the role's\n      permissions; admins can switch a role to \"Customize for AI\" and restrict it further. AI\n      permissions can never exceed the role's own non-Kubernetes permissions, so an agent is\n      always capped at what the user it acts for could already do, or less.\n    since:\
  \ v0.92\n    source: https://www.facets.cloud/docs/changelog/release-notes-v092\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facets/refs/heads/main/authentication/facets-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Infrastructure
- Orchestration
- Platform Engineering
- DevOps
- Internal Developer Platform
- Terraform
- Kubernetes
- Continuous Delivery
- AI Agents
---
