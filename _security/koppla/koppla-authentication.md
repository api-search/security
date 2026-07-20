---
api_key_in: []
auth_types:
- bearer
description: ''
kind: authentication
layout: security
method: derived
name: Koppla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koppla secures its APIs with bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Koppla
provider_slug: koppla
scheme_count: 1
schemes:
- enforced: true
  evidence: POST https://api.koppla.de/api/graphql/v1 with {"query":"{ownUser{id}}"} and no credentials returns errors[0].extensions.code = UNAUTHENTICATED with message "Invalid Authentication".
  name: bearer
  scheme: bearer
  sources:
  - graphql/koppla-graphql-introspection.json
  type: http
slug: koppla-authentication
source_filename: koppla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: graphql/koppla-graphql-introspection.json + live probes of api.koppla.de\ndocs: null\ndocs_note: koppla publishes no public authentication documentation; the API is an\n  Enterprise contract feature.\nsummary:\n  types:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  spec_declared: false\n  spec_note: 'GraphQL has no securitySchemes construct, so the auth model here is\n    derived from observed responses and the published web client, not from a formal\n    declaration.'\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  enforced: true\n  evidence: 'POST https://api.koppla.de/api/graphql/v1 with {\"query\":\"{ownUser{id}}\"}\n    and no credentials returns errors[0].extensions.code = UNAUTHENTICATED with\n    message \"Invalid Authentication\".'\n  sources:\n  - graphql/koppla-graphql-introspection.json\nidentity_provider:\n  name: WorkOS\n  role: authentication / SSO for the koppla web application\n  evidence:\
  \ 'https://my.koppla.de/sign_in loads\n    /assets/workosAuthenticationService-CqIsie4P.js alongside\n    useAuthenticationService-*.js.'\n  confidence: high\n  caveat: Inferred from the public web client bundle; koppla does not publish this.\nsso:\n  advertised: true\n  source: https://security.koppla.de/\n  detail: Single-Sign-On (SSO) is listed as an Access Control capability on the koppla\n    trust center.\naccess_control:\n  model: role-based\n  advertised: Role-Based Access Control (koppla trust center, Product Security)\n  schema_roles:\n    enum: MembershipRole\n    values:\n    - ADMIN\n    - CONTROLLER\n    - MEMBER\n  tenancy: 'Multi-tenant. Many root queries require a tenant: ID! argument (for\n    example projects(tenant: ID!)), and organizationalUnit / membership types scope\n    access within a tenant.'\n  credential_management: listed as an App Security control on the koppla trust center\nintrospection:\n  enabled: true\n  authenticated: false\n  note: 'GraphQL schema\
  \ introspection is answered without credentials on the\n    production endpoint, which is how this repo captured the schema. Data access is\n    correctly gated - only the schema shape is exposed. Disabling production\n    introspection (or gating it behind auth) is the conventional hardening choice;\n    recorded here as an observation, not a vulnerability report.'\nhosts:\n- host: api.koppla.de\n  role: GraphQL API\n  gateway: AWS API Gateway\n  unauthenticated_response: '{\"message\":\"Missing Authentication Token\"} (HTTP 403) on\n    non-GraphQL paths'\n- host: api-v2.koppla.de\n  role: REST API (referenced by web client config and by in-schema deprecation notes)\n  reachable_unauthenticated: false\n- host: bulk.koppla.de\n  role: bulk endpoint (/v1)\n  unauthenticated_response: HTTP 403\n- host: rtc.koppla.de\n  role: realtime websocket (wss)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koppla/refs/heads/main/authentication/koppla-authentication.yml
summary_line: bearer · 1 scheme
tags:
- Company
- Construction
- Construction Technology
- Project Management
- Scheduling
- Lean Construction
- BIM
- Germany
- SaaS
---
