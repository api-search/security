---
api_key_in:
- header
api_specs:
- filename: kondukto-aspm-openapi.yml
  format: yaml
  label: Invicti ASPM (Kondukto) REST API v2
  slug: aspm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-aspm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kondukto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kondukto secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kondukto
provider_slug: kondukto
scheme_count: 1
schemes:
- description: Kondukto-issued Personal Access Token. Every authenticated request to the Kondukto API must include the X-Cookie header carrying the token value.
  in: header
  name: apiToken
  parameter_name: X-Cookie
  provisioning:
    docs: https://docs.kondukto.io/reference/get-api-token-via-ui
    method: ui
    steps:
    - Log in to Invicti ASPM.
    - Go to Integrations > Personal Access Token (labelled API Tokens in newer releases).
    - Select Generate Token and copy the value.
    warning: The token is displayed only once and cannot be retrieved again.
  rotation:
    note: No documented expiry or automated rotation policy for API tokens.
    policy_published: false
  sources:
  - openapi/kondukto-aspm-openapi.yml
  type: apiKey
  used_by:
  - client: KDT CLI
    legacy_mechanism: KONDUKTO_TOKEN (deprecated, still supported)
    mechanism: INVICTI_ASPM_TOKEN environment variable, --token flag, or token key in $HOME/.kdt.yaml
slug: kondukto-authentication
source_filename: kondukto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kondukto-aspm-openapi.yml\ndocs: https://docs.kondukto.io/reference/starting-with-kondukto-api\ntoken_docs: https://docs.kondukto.io/reference/get-api-token-via-ui\nnotes: >-\n  Invicti ASPM (Kondukto) authenticates the public REST API v2 with a single long-lived, user-scoped\n  API token sent in a custom X-Cookie request header. There is no OAuth 2.0, OpenID Connect or\n  mutual-TLS surface on the public API, so no scopes/ artifact applies: authorization is enforced by\n  the token owner's role and team membership rather than by token scopes. SSO (Okta, Azure AD SAML\n  2.0, Google Workspace SAML 2.0) governs interactive user sign-in to the platform, not API calls.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_names: [X-Cookie]\n  oauth2_flows: []\n  scoped: false\n  authorization_model: role-and-team based (see user permission matrix)\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter_name:\
  \ X-Cookie\n  description: >-\n    Kondukto-issued Personal Access Token. Every authenticated request to the Kondukto API must\n    include the X-Cookie header carrying the token value.\n  sources: [openapi/kondukto-aspm-openapi.yml]\n  provisioning:\n    method: ui\n    steps:\n    - Log in to Invicti ASPM.\n    - Go to Integrations > Personal Access Token (labelled API Tokens in newer releases).\n    - Select Generate Token and copy the value.\n    warning: The token is displayed only once and cannot be retrieved again.\n    docs: https://docs.kondukto.io/reference/get-api-token-via-ui\n  rotation:\n    policy_published: false\n    note: No documented expiry or automated rotation policy for API tokens.\n  used_by:\n  - client: KDT CLI\n    mechanism: INVICTI_ASPM_TOKEN environment variable, --token flag, or token key in $HOME/.kdt.yaml\n    legacy_mechanism: KONDUKTO_TOKEN (deprecated, still supported)\nunauthenticated_operations:\n- operationId: health-check\n  path: /api/v2/health/check/\n\
  \  note: Published with an empty security requirement in the provider's own OpenAPI definition.\nfailure_responses:\n- status: 401\n  body: '{\"error\": \"failed to authorize\"}'\n  meaning: Missing, malformed or revoked token.\n- status: 403\n  body: '{\"message\": \"forbidden operation\"}'\n  meaning: Valid token whose owner lacks permission for the resource.\nwebhook_authentication:\n  outbound:\n    description: >-\n      Outbound webhooks support user-defined custom HTTP headers plus a \"Secure\" mode toggle\n      configured per webhook in Integrations > Webhooks.\n    docs: https://docs.kondukto.io/docs/webhook-integration-capturing-audit-log-events\n  issue_manager:\n    description: >-\n      Kondukto authenticates itself to a customer-hosted webhook issue manager with a shared secret\n      in the X-Kondukto-Secret header; a missing header returns 403 \"missing secret key\".\n    header: X-Kondukto-Secret\n    docs: https://docs.kondukto.io/docs/integrating-with-webhooks\nsso:\n\
  \  applies_to: interactive platform sign-in only, not the REST API\n  providers:\n  - name: Okta\n    docs: https://docs.kondukto.io/docs/okta\n  - name: Azure AD (SAML 2.0)\n    docs: https://docs.kondukto.io/docs/saml-20-azure-ad-integration\n  - name: Google Workspace (SAML 2.0)\n    docs: https://docs.kondukto.io/docs/saml-20-google-workspace-integration\n  discovery_endpoint: https://docs.kondukto.io/reference/get-active-auth-managers\nauthorization:\n  model: role and team based\n  docs: https://docs.kondukto.io/docs/user-permission-matrix\n  roles_docs: https://docs.kondukto.io/docs/roles\nrelated:\n  conventions: conventions/kondukto-conventions.yml\n  errors: errors/kondukto-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/authentication/kondukto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Application Security
- ASPM
- Vulnerability Management
- DevSecOps
- Security Orchestration
- SAST
- DAST
- SCA
- Software Composition Analysis
- Container Security
- SBOM
- Security Testing
- CI/CD
- Security
---
