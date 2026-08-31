---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Stacklet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stacklet declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Stacklet
provider_slug: stacklet
scheme_count: 3
schemes:
- description: Browser-based single sign-on, brokered by AWS Cognito against the customer's identity provider. `stacklet-admin login` with no arguments opens a browser, completes the SSO flow, and writes the resulting access and identity tokens to ~/.stacklet/credentials and ~/.stacklet/id.
  flow: authorization_code
  id: sso
  identity_provider: AWS Cognito user pool, per deployment
  session_lifetime: 12 hours (as used by the MCP server)
  type: oauth2
- description: '`stacklet-admin login --username <user>` bypasses SSO and prompts for a password; `--password` is available but the docs call it out as less secure because it leaks through shell history and process listings.'
  flow: password
  id: password
  type: oauth2
- description: Non-interactive API key. The CLI reads it from STACKLET_API_KEY and skips the login step entirely; the Terraform provider takes it as the `api_key` argument or the same environment variable. The provider changelog records that the `Bearer` type was added to the Authorization header in 0.6.1 (2026-01-23).
  env: STACKLET_API_KEY
  header: Authorization
  id: api_key
  in: header
  scheme: Bearer
  type: apiKey
slug: stacklet-authentication
source_filename: stacklet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://github.com/stacklet/stacklet-admin#readme, https://github.com/stacklet/terraform-provider-stacklet#readme,\n  https://github.com/stacklet/mcp-server/blob/main/stacklet/mcp/stacklet_auth.py\nnote: 'No OpenAPI exists to derive securitySchemes from; this profile is read from the\n  provider''s own first-party clients, which are the published description of how the\n  Platform GraphQL API is authenticated.'\napi: Stacklet Platform API\nendpoint: https://api.{instance}.stacklet.io/\nschemes:\n- id: sso\n  type: oauth2\n  flow: authorization_code\n  description: 'Browser-based single sign-on, brokered by AWS Cognito against the\n    customer''s identity provider. `stacklet-admin login` with no arguments opens a\n    browser, completes the SSO flow, and writes the resulting access and identity tokens\n    to ~/.stacklet/credentials and ~/.stacklet/id.'\n  session_lifetime: 12 hours (as used by the MCP server)\n  identity_provider:\
  \ AWS Cognito user pool, per deployment\n- id: password\n  type: oauth2\n  flow: password\n  description: '`stacklet-admin login --username <user>` bypasses SSO and prompts for a\n    password; `--password` is available but the docs call it out as less secure because\n    it leaks through shell history and process listings.'\n- id: api_key\n  type: apiKey\n  in: header\n  header: Authorization\n  scheme: Bearer\n  env: STACKLET_API_KEY\n  description: 'Non-interactive API key. The CLI reads it from STACKLET_API_KEY and skips\n    the login step entirely; the Terraform provider takes it as the `api_key` argument or\n    the same environment variable. The provider changelog records that the `Bearer` type\n    was added to the Authorization header in 0.6.1 (2026-01-23).'\ncredential_sources:\n  order:\n  - Environment variables — STACKLET_ENDPOINT, STACKLET_ACCESS_TOKEN, STACKLET_IDENTITY_TOKEN\n  - ~/.stacklet/config.json (the `api` key holds the endpoint)\n  - ~/.stacklet/credentials (access\
  \ token)\n  - ~/.stacklet/id (identity token)\n  note: The Terraform provider and the MCP server both fall back to the credentials\n    written by the stacklet-admin CLI, so a single interactive login authenticates all\n    three clients.\ntokens:\n- name: access_token\n  header: Authorization\n  scheme: Bearer\n- name: identity_token\n  note: Sent alongside the access token; carried in the credentials tuple used by every\n    first-party client.\nservice_endpoints:\n  pattern: 'The first `api.` label of the endpoint is replaced with the service name —\n    api.<instance>.stacklet.io becomes docs.<instance>.stacklet.io for documentation.'\n  source: stacklet/mcp/stacklet_auth.py StackletCredentials.service_endpoint\nauthorization:\n  model: 'Stacklet users carry roles and role assignments (stacklet_role,\n    stacklet_role_assignment, stacklet_sso_group in the Terraform provider); the MCP\n    server documentation recommends creating a purpose-scoped user rather than reusing an\n    operator\
  \ account.'\n  scopes_published: false\n  note: No OAuth scope reference is published on any public Stacklet surface, so no\n    scopes/ artifact is emitted.\ngaps:\n- No public authentication reference page — every detail here comes from first-party\n  client repositories rather than a hosted docs site.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is\n  served on any publicly resolvable Stacklet host (both 404 on stacklet.ai and\n  stacklet.io); the Cognito discovery document lives inside each customer deployment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacklet/refs/heads/main/authentication/stacklet-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Cloud Governance
- Cloud Custodian
- Policy as Code
- FinOps
- Cloud Security
- Compliance
- Infrastructure as Code
- Terraform
- GraphQL
- Model Context Protocol
- Azure
- Google Cloud
- Agents
---
