---
api_key_in: []
api_specs:
- filename: infra-openapi-original.json
  format: json
  label: Infra API
  slug: infra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-openapi-original.json
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Infra Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Infra secures its APIs with http-bearer across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Infra
provider_slug: infra
scheme_count: 4
schemes:
- description: 'All authenticated requests send Authorization: Bearer <ACCESSKEY>. Access keys are organization-scoped and inherit the permissions of the identity that created them. Keys carry an expiry and inactivity timeout.'
  name: accessKey
  scheme: bearer
  sources:
  - https://github.com/infrahq/infra/blob/main/docs/reference/api.md
  type: http
- description: Required on every request; pins the API contract version (e.g. 0.18.1). Not a credential, but mandatory alongside the bearer access key.
  in: header
  name: infraVersionHeader
  parameter_name: Infra-Version
  type: apiKey
- description: Interactive login via a configured OIDC identity provider (Okta, Google, Azure AD, etc.). POST /api/login with an `oidc` credential (providerID, code, redirectURL); also supports the OAuth2 device authorization flow (/api/device).
  name: oidcLogin
  type: openIdConnect
- description: POST /api/login with `passwordCredentials` (name + password) for local identities; includes password reset endpoints.
  name: passwordLogin
  scheme: basic
  type: http
slug: infra-authentication
source_filename: infra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/infrahq/infra/blob/main/docs/reference/api.md\ndocs: https://github.com/infrahq/infra/blob/main/docs/reference/api.md\nnote: The OpenAPI document does not declare formal securitySchemes; this profile is\n  captured from the documented API reference.\nsummary:\n  types:\n  - http-bearer\n  api_key_in: []\n  oauth2_flows:\n  - deviceCode\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'All authenticated requests send Authorization: Bearer <ACCESSKEY>.\n    Access keys are organization-scoped and inherit the permissions of the identity\n    that created them. Keys carry an expiry and inactivity timeout.'\n  sources:\n  - https://github.com/infrahq/infra/blob/main/docs/reference/api.md\n- name: infraVersionHeader\n  type: apiKey\n  in: header\n  parameter_name: Infra-Version\n  description: Required on every request; pins the API contract version (e.g. 0.18.1).\n    Not a credential,\
  \ but mandatory alongside the bearer access key.\n- name: oidcLogin\n  type: openIdConnect\n  description: Interactive login via a configured OIDC identity provider (Okta, Google,\n    Azure AD, etc.). POST /api/login with an `oidc` credential (providerID, code,\n    redirectURL); also supports the OAuth2 device authorization flow (/api/device).\n- name: passwordLogin\n  type: http\n  scheme: basic\n  description: POST /api/login with `passwordCredentials` (name + password) for local\n    identities; includes password reset endpoints.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/authentication/infra-authentication.yml
summary_line: http-bearer · 4 schemes
tags:
- Company
- Identity
- Access Management
- Authentication
- Authorization
- Infrastructure
- Kubernetes
- OIDC
- Security
- Open Source
---
