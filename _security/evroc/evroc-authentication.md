---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Evroc Authentication
name_suffix: Authentication
oauth_flows:
- oidc
overview: evroc secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the oidc flow(s).
provider_name: evroc
provider_slug: evroc
scheme_count: 3
schemes:
- description: 'REST API requests carry an "Authorization: Bearer {token}" header. Access tokens are obtained via the CLI (evroc iam get-access-token / evroc login) or the documented Python OIDC flow, and expire after 5 minutes.'
  name: bearerToken
  scheme: bearer
  sources:
  - https://docs.evroc.com/gettingstarted.html
  type: http
- description: Access tokens are issued through an OpenID Connect flow against the evroc IAM authorization server. evroc publishes an example Python OIDC script for programmatic token acquisition.
  name: oidc
  sources:
  - https://docs.evroc.com/products/iam/authentication.html
  type: openIdConnect
- description: Non-interactive workloads authenticate with service-account credentials supplied as environment variables (EVROC_USERNAME, EVROC_PASSWORD, EVROC_PROJECT, EVROC_REGION) which the SDK/CLI exchange for a Bearer access token.
  name: serviceAccount
  scheme: basic
  sources:
  - https://github.com/evroc-oss/evroc-go-sdk
  type: http
slug: evroc-authentication
source_filename: evroc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.evroc.com/products/iam/authentication.html\ndocs: https://docs.evroc.com/products/iam/authentication.html\nsummary:\n  types: [oauth2, http]\n  http_scheme: bearer\n  oauth2_flows: [oidc]\n  token_ttl_seconds: 300\n  api_key_in: []\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    REST API requests carry an \"Authorization: Bearer {token}\" header. Access tokens are obtained\n    via the CLI (evroc iam get-access-token / evroc login) or the documented Python OIDC flow, and\n    expire after 5 minutes.\n  sources: [https://docs.evroc.com/gettingstarted.html]\n- name: oidc\n  type: openIdConnect\n  description: >-\n    Access tokens are issued through an OpenID Connect flow against the evroc IAM authorization\n    server. evroc publishes an example Python OIDC script for programmatic token acquisition.\n  sources: [https://docs.evroc.com/products/iam/authentication.html]\n- name:\
  \ serviceAccount\n  type: http\n  scheme: basic\n  description: >-\n    Non-interactive workloads authenticate with service-account credentials supplied as environment\n    variables (EVROC_USERNAME, EVROC_PASSWORD, EVROC_PROJECT, EVROC_REGION) which the SDK/CLI\n    exchange for a Bearer access token.\n  sources: [https://github.com/evroc-oss/evroc-go-sdk]\nconsole_auth:\n  method: email-password\n  mfa: TOTP (optional, strongly recommended)\n  description: >-\n    Human console access at cloud.evroc.com uses email + password with optional time-based one-time\n    password (TOTP) multi-factor authentication.\nauthorization:\n  model: RoleBindings\n  description: >-\n    Fine-grained permission system (released 2026-07-15) that assigns roles to identities via\n    RoleBindings, replacing the deprecated PermissionSets. Scoped to organizations and projects.\n  deprecated: [PermissionSets]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evroc/refs/heads/main/authentication/evroc-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Cloud Computing
- Sovereign Cloud
- Infrastructure
- Object Storage
- Compute
- AI Infrastructure
- GPU
- Europe
- IaaS
---
