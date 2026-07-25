---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kubit Ai Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubit AI, Inc. declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Kubit AI, Inc.
provider_slug: kubit-ai-inc
scheme_count: 3
schemes:
- dynamic_client_registration:
    registration_endpoint: https://mcp.kubit.ai/auth/oauth2/register
    supported: true
  flows:
    authorization_code:
      authorization_url: https://mcp.kubit.ai/auth/oauth2/authorize
      pkce_methods:
      - S256
      refresh_supported: true
      scopes:
      - mcp:read
      - mcp:write
      token_url: https://mcp.kubit.ai/auth/oauth2/token
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp_oauth2
  issuer: https://mcp.kubit.ai
  response_types:
  - code
  surface: https://mcp.kubit.ai/mcp
  type: oauth2
- description: 'Single Sign-On for the Kubit web platform. Documented identity providers: Google Workspace, Okta, Azure Microsoft Entra ID (Active Directory), and AWS IAM Identity Center. SSO LDAP groups can be synced to Kubit groups.'
  id: platform_sso
  providers:
  - docs: https://docs.kubit.ai/docs/google-workspace
    name: Google Workspace
  - docs: https://docs.kubit.ai/docs/okta
    name: Okta
  - docs: https://docs.kubit.ai/docs/azure-active-directory-ad
    name: Azure Microsoft Entra ID
  - docs: https://docs.kubit.ai/docs/aws-iam-identity-center
    name: AWS IAM Identity Center
  surface: https://app.kubit.ai
  type: openIdConnect
- description: 'Fallback for organizations without SSO: an invite email issues a temporary password; the user then sets a permanent password and enrolls in multi-factor authentication.'
  id: platform_password
  mfa: true
  scheme: basic-invite
  type: http
slug: kubit-ai-inc-authentication
source_filename: kubit-ai-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kubit.ai/docs/mcp-server + https://mcp.kubit.ai/.well-known/oauth-authorization-server\ndocs:\n  - https://docs.kubit.ai/docs/single-sign-on-sso\n  - https://docs.kubit.ai/docs/login-to-kubit\n  - https://docs.kubit.ai/docs/mcp-server\nsummary: >-\n  Kubit has no public API-key surface. Programmatic access is the hosted MCP server,\n  which is protected by OAuth 2.1 authorization code with PKCE and supports dynamic\n  client registration. Human access to the Kubit web platform is SSO-first, with\n  invite-email plus password and MFA as the fallback.\nschemes:\n  - id: mcp_oauth2\n    type: oauth2\n    surface: https://mcp.kubit.ai/mcp\n    flows:\n      authorization_code:\n        authorization_url: https://mcp.kubit.ai/auth/oauth2/authorize\n        token_url: https://mcp.kubit.ai/auth/oauth2/token\n        refresh_supported: true\n        pkce_methods:\n          - S256\n        scopes:\n          - mcp:read\n\
  \          - mcp:write\n    dynamic_client_registration:\n      supported: true\n      registration_endpoint: https://mcp.kubit.ai/auth/oauth2/register\n    issuer: https://mcp.kubit.ai\n    response_types:\n      - code\n    grant_types:\n      - authorization_code\n      - refresh_token\n  - id: platform_sso\n    type: openIdConnect\n    surface: https://app.kubit.ai\n    description: >-\n      Single Sign-On for the Kubit web platform. Documented identity providers:\n      Google Workspace, Okta, Azure Microsoft Entra ID (Active Directory), and\n      AWS IAM Identity Center. SSO LDAP groups can be synced to Kubit groups.\n    providers:\n      - name: Google Workspace\n        docs: https://docs.kubit.ai/docs/google-workspace\n      - name: Okta\n        docs: https://docs.kubit.ai/docs/okta\n      - name: Azure Microsoft Entra ID\n        docs: https://docs.kubit.ai/docs/azure-active-directory-ad\n      - name: AWS IAM Identity Center\n        docs: https://docs.kubit.ai/docs/aws-iam-identity-center\n\
  \  - id: platform_password\n    type: http\n    scheme: basic-invite\n    description: >-\n      Fallback for organizations without SSO: an invite email issues a temporary\n      password; the user then sets a permanent password and enrolls in multi-factor\n      authentication.\n    mfa: true\nauthorization:\n  model: rbac\n  docs: https://docs.kubit.ai/docs/kubit-user-roles-and-permissions\n  built_in_roles:\n    - Admin\n    - Governor\n    - Creator\n    - Viewer\n  notes: >-\n    Custom roles with granular permissions and schema-specific access are supported;\n    MCP tool calls are evaluated against the same role-based access controls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubit-ai-inc/refs/heads/main/authentication/kubit-ai-inc-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Analytics
- Product Analytics
- Data Warehouse
- LLM Observability
- Model Context Protocol
- Agent Analytics
- OpenTelemetry
- Devops
---
