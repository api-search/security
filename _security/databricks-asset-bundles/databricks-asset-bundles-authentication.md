---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Databricks Asset Bundles Authentication
name_suffix: Authentication
oauth_flows: []
overview: Databricks Asset Bundles declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Databricks Asset Bundles
provider_slug: databricks-asset-bundles
scheme_count: 4
schemes:
- authorization_endpoint: https://accounts.cloud.databricks.com/oidc/v1/authorize
  description: '`databricks auth login` runs the browser authorization-code flow and writes a Databricks configuration profile automatically. This is the method the bundle documentation names first.'
  flow: authorization_code
  id: oauth-u2m
  label: OAuth user-to-machine (U2M)
  pkce: S256
  recommended_for: attended / interactive bundle work
  token_endpoint: https://accounts.cloud.databricks.com/oidc/v1/token
  type: oauth2
- description: A service principal's client ID and secret exchanged at the token endpoint. The bundle documentation names this the preferred unattended method because "CI/CD systems are typically optimized for" environment variables.
  flow: client_credentials
  id: oauth-m2m
  label: OAuth machine-to-machine (M2M)
  recommended_for: unattended / CI/CD bundle deployment
  token_endpoint: https://accounts.cloud.databricks.com/oidc/v1/token
  type: oauth2
- description: A Databricks personal access token, for a user or for a service principal. The documentation classes it as the legacy alternative to OAuth for both attended and unattended scenarios.
  id: pat
  label: Personal access token
  scheme: bearer
  status: legacy
  type: http
- description: Credentials stored locally in ~/.databrickscfg and selected per command with `-p` / `--profile`, letting a developer "quickly switch among different Databricks authentication contexts" without editing the bundle.
  id: config-profile
  label: Databricks configuration profile
  selector_flags:
  - -p
  - --profile
  type: local-credential-store
slug: databricks-asset-bundles-authentication
source_filename: databricks-asset-bundles-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.databricks.com/aws/en/dev-tools/bundles/authentication\ndocs: https://docs.databricks.com/aws/en/dev-tools/bundles/authentication\nprobe_evidence:\n  - url: https://accounts.cloud.databricks.com/oidc/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://accounts.cloud.databricks.com/oidc/.well-known/openid-configuration\n    status: 200\nnote: >-\n  There is no OpenAPI for this product to derive securitySchemes from\n  (derive-authentication.py found zero schemes because no spec exists). This\n  profile is read from the provider's own bundle-authentication documentation\n  and from the RFC 8414 authorization server metadata Databricks serves\n  anonymously.\nsummary: >-\n  Declarative Automation Bundles never carry credentials in databricks.yml.\n  Authentication is resolved by the Databricks CLI through the unified\n  Databricks client authentication chain — a named configuration profile, or\n\
  \  environment variables — and the recommended methods are OAuth U2M for\n  attended work and OAuth M2M (service principal) for CI/CD.\nschemes:\n  - id: oauth-u2m\n    type: oauth2\n    flow: authorization_code\n    pkce: S256\n    label: OAuth user-to-machine (U2M)\n    recommended_for: attended / interactive bundle work\n    description: >-\n      `databricks auth login` runs the browser authorization-code flow and\n      writes a Databricks configuration profile automatically. This is the\n      method the bundle documentation names first.\n    authorization_endpoint: https://accounts.cloud.databricks.com/oidc/v1/authorize\n    token_endpoint: https://accounts.cloud.databricks.com/oidc/v1/token\n  - id: oauth-m2m\n    type: oauth2\n    flow: client_credentials\n    label: OAuth machine-to-machine (M2M)\n    recommended_for: unattended / CI/CD bundle deployment\n    description: >-\n      A service principal's client ID and secret exchanged at the token\n      endpoint. The bundle documentation\
  \ names this the preferred unattended\n      method because \"CI/CD systems are typically optimized for\" environment\n      variables.\n    token_endpoint: https://accounts.cloud.databricks.com/oidc/v1/token\n  - id: pat\n    type: http\n    scheme: bearer\n    label: Personal access token\n    status: legacy\n    description: >-\n      A Databricks personal access token, for a user or for a service\n      principal. The documentation classes it as the legacy alternative to\n      OAuth for both attended and unattended scenarios.\n  - id: config-profile\n    type: local-credential-store\n    label: Databricks configuration profile\n    description: >-\n      Credentials stored locally in ~/.databrickscfg and selected per command\n      with `-p` / `--profile`, letting a developer \"quickly switch among\n      different Databricks authentication contexts\" without editing the bundle.\n    selector_flags:\n      - -p\n      - --profile\ntarget_binding:\n  description: >-\n    A bundle target\
  \ can pin the workspace host and the profile it authenticates\n    with, so `databricks bundle deploy -t prod` resolves credentials for that\n    environment rather than whatever the shell happens to hold.\n  fields:\n    - targets.<name>.workspace.host\n    - targets.<name>.workspace.profile\n    - targets.<name>.workspace.auth_type\n    - run_as\nscopes_reference: ../scopes/databricks-asset-bundles-scopes.yml\ngaps:\n  - >-\n    The bundle authentication page defers the exact environment-variable names\n    and OAuth scopes to the general Databricks authorization guides rather than\n    naming them inline; they are not restated here as if the bundle page said\n    them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databricks-asset-bundles/refs/heads/main/authentication/databricks-asset-bundles-authentication.yml
summary_line: 4 schemes
tags:
- CI/CD
- Data Engineering
- Databricks
- Deployment
- Infrastructure as Code
- Job
- Machine-Learning
- MLOps
- Pipelines
- Workflows
---
