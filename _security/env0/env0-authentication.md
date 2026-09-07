---
anonymous_access: false
api_key_in: []
api_specs:
- filename: env0-agents-api-openapi.yml
  format: yaml
  label: Env0 Agents API
  slug: env0-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-agents-api-openapi.yml
- filename: env0-approvalpolicies-api-openapi.yml
  format: yaml
  label: Env0 ApprovalPolicies API
  slug: env0-approvalpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-approvalpolicies-api-openapi.yml
- filename: env0-configuration-api-openapi.yml
  format: yaml
  label: Env0 Configuration API
  slug: env0-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-configuration-api-openapi.yml
- filename: env0-deployments-api-openapi.yml
  format: yaml
  label: Env0 Deployments API
  slug: env0-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-deployments-api-openapi.yml
- filename: env0-environments-api-openapi.yml
  format: yaml
  label: Env0 Environments API
  slug: env0-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-environments-api-openapi.yml
- filename: env0-modules-api-openapi.yml
  format: yaml
  label: Env0 Modules API
  slug: env0-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-modules-api-openapi.yml
- filename: env0-organizations-api-openapi.yml
  format: yaml
  label: Env0 Organizations API
  slug: env0-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-organizations-api-openapi.yml
- filename: env0-projects-api-openapi.yml
  format: yaml
  label: Env0 Projects API
  slug: env0-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-projects-api-openapi.yml
- filename: env0-templates-api-openapi.yml
  format: yaml
  label: Env0 Templates API
  slug: env0-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-templates-api-openapi.yml
- filename: env0-users-api-openapi.yml
  format: yaml
  label: Env0 Users API
  slug: env0-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-users-api-openapi.yml
- filename: env0-webhooks-api-openapi.yml
  format: yaml
  label: Env0 Webhooks API
  slug: env0-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Env0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Env0 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Env0
provider_slug: env0
scheme_count: 1
schemes:
- applies_to: https://api.env0.com (all published operations)
  description: HTTP Basic Authentication. Username is the env zero API Key ID, password is the API Key Secret. Both are created in Organization Settings -> API Keys.
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.envzero.com/guides/admin-guide/user-role-and-team-management/api-keys
  type: http
slug: env0-authentication
source_filename: env0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.envzero.com/guides/admin-guide/user-role-and-team-management/api-keys\ndocs: https://docs.envzero.com/guides/admin-guide/user-role-and-team-management/api-keys\nnote: >-\n  Upgraded from derived to searched 2026-09-06 against env zero's own documentation. The REST API\n  uses HTTP Basic only - API Key ID as username, API Key Secret as password. There is no OAuth\n  authorization server, no bearer token endpoint and no scope vocabulary for the API, so no\n  scopes/ artifact is written; RBAC is attached to the KEY, not to the token.\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  scoped_tokens: false\n  rbac: true\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Username is the env zero API Key ID, password is the API\n    Key Secret. Both are created in Organization Settings -> API Keys.\n  sources: [https://docs.envzero.com/guides/admin-guide/user-role-and-team-management/api-keys]\n\
  \  applies_to: https://api.env0.com (all published operations)\ncredentials:\n  key_types:\n  - name: Admin API key\n    permissions: any request requiring admin permission - organization settings, deploying and\n      approving environments\n    default: true\n  - name: User (non-admin) API key\n    permissions: RBAC-scoped - specific project permissions, team assignment, treated like any\n      other user\n  - name: Personal API key\n    permissions: the same permissions the issuing user has in their env zero account\n    self_serve: true\n    note: every user can generate one\n  creation: Organization Settings -> API Keys, or POST /api-keys\n  secret_visibility: shown once at creation; not retrievable afterwards\n  revocation: deleting a key can take up to 1 hour to fully expire\n  rotation_policy: none published\n  expiry: none published\nenvironment_variables:\n  cli_and_ci:\n  - ENV0_API_KEY_ID\n  - ENV0_API_SECRET\n  mcp_server:\n  - ENV0_API_KEY\n  - ENV0_API_SECRET\n  - ENV0_ORGANIZATION_ID\n\
  \  note: >-\n    The variable names are NOT consistent across env zero's own tooling. The CLI v2 reads\n    ENV0_API_KEY_ID (renamed from ENV0_API_KEY in the v1 -> v2 migration) while the official MCP\n    server README still uses ENV0_API_KEY. Both are current provider documentation as of\n    2026-09-06.\nother_authentication_surfaces:\n- name: SCIM bearer token\n  type: http\n  scheme: bearer\n  applies_to: the per-organization SCIM 2.0 endpoint (/scim/v2/*)\n  issuance: generated in Organization Settings -> SSO -> SCIM Provisioning\n  visibility: shown once\n  rotation: supported; the previous token stays valid for a grace window (default 24h) then is revoked\n  revocation: deleting the SCIM configuration revokes immediately\n  operations: [GET/POST/DELETE SCIM Configuration, Rotate SCIM Token, Update SCIM Mode, Reconcile SCIM State]\n- name: OIDC (outbound)\n  type: openIdConnect\n  direction: env zero is the ISSUER\n  applies_to: workload identity from a deployment to AWS, Azure,\
  \ GCP or HashiCorp Vault\n  detail: since July 2026 the token audience can be per-cloud-provider rather than one shared audience\n  docs: https://docs.envzero.com/guides/integrations/oidc-integrations\n- name: SSO (human sign-in)\n  type: saml2 / oidc\n  providers: [SAML 2.0 (Okta, OneLogin, Google Workspace, JumpCloud), Azure AD / Microsoft Entra ID]\n  self_service: true\n  docs: https://docs.envzero.com/guides/sso-integrations/self-service-sso\n- name: VCS OAuth\n  type: oauth2\n  direction: env zero is the CLIENT\n  applies_to: GitHub.com, GitLab.com, Bitbucket.org connections\n  self_hosted_alternative: SSH keys or HTTPS access tokens\n- name: Agent access token\n  applies_to: self-hosted Kubernetes or standalone Docker agent registration\n  docs: https://docs.envzero.com/guides/admin-guide/self-hosted-kubernetes-agent/overview\n- name: Agent secrets\n  applies_to: per-agent secrets, created once and revocable (\"immediate and irreversible\")\nnetwork_controls:\n  ip_allowlisting:\n\
  \    available: true\n    scope: per-organization - UI logins, API keys and the Agent API\n    protocols: [IPv4, IPv6, subnets]\n    default: no allowlist means all IPs allowed\n    enablement: contact the env zero account team or support\n    docs: https://docs.envzero.com/changelogs/2026/05/ip-allowlisting\n  egress_ips_published: true\n  egress_ips_docs: https://docs.envzero.com/guides/admin-guide/custom-flows#faq\ndiscovery:\n  openid_configuration: absent\n  oauth_authorization_server: absent\n  oauth_protected_resource: absent\n  probed: '2026-09-06'\n  probed_hosts: [env0.com, www.env0.com, envzero.com, www.envzero.com, api.env0.com, docs.envzero.com, app.env0.com, status.env0.com]\n  see: well-known/env0-well-known.yml\nunauthenticated_behavior:\n  url: https://api.env0.com/\n  status: 403\n  body: '{\"message\":\"Missing Authentication Token\"}'\n  note: the AWS API Gateway default response, not an env zero error contract. It returns the same\n    body for every path, so a 403\
  \ here does not distinguish a real endpoint from one that does\n    not exist.\n  fetched: '2026-09-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/authentication/env0-authentication.yml
summary_line: http · 1 scheme
tags:
- FinOps
- Infrastructure as Code
- DevOps
- Cloud
- Terraform
- OpenTofu
- Platform Engineering
- Cloud Governance
- Drift Detection
---
