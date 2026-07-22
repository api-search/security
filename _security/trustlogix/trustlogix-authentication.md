---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Trustlogix Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Trustlogix secures its APIs with apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Trustlogix
provider_slug: trustlogix
scheme_count: 4
schemes:
- applies_to: TrustLogix REST API (/api/*)
  description: REST API requests authenticate with an API key passed in the Authorization header. Most tenant-scoped endpoints additionally require a tenantId header.
  in: header
  name: ApiKeyAuth
  parameter_name: Authorization
  source: https://docs.trustlogix.io/trustlogix-api-documentation.md
  type: apiKey
- description: POST /api/login exchanges loginId + password (+ optional TOTP for MFA) for a session; POST /api/logout ends it.
  name: SessionLogin
  scheme: custom
  source: https://docs.trustlogix.io/trustlogix-api-documentation.md
  type: http
- description: The TrustAI MCP Server authorizes agent connections with OAuth 2.0, implementing RFC 9728 Protected Resource Metadata per the MCP Authentication Specification. End-user OAuth tokens are propagated in the Authorization header to carry end-user identity to the policy engine.
  flow: authorizationCode
  name: MCP-OAuth2
  source: https://docs.trustlogix.io/trust-ai/mcp-server.md
  standards:
  - RFC9728
  type: oauth2
- description: Console/tenant single sign-on via Azure Active Directory (MS Entra) and Okta, with SCIM 2.0 user provisioning/deprovisioning and a regenerable SCIM token.
  identity_providers:
  - Azure AD / MS Entra
  - Okta
  name: SSO-OIDC
  provisioning: SCIM 2.0
  source: https://docs.trustlogix.io/integrations/single-sign-on.md
  type: openIdConnect
slug: trustlogix-authentication
source_filename: trustlogix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.trustlogix.io/trustlogix-api-documentation.md\ndocs:\n  - https://docs.trustlogix.io/trustlogix-api-documentation.md\n  - https://docs.trustlogix.io/integrations/single-sign-on.md\n  - https://docs.trustlogix.io/trust-ai/mcp-server.md\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    description: >-\n      REST API requests authenticate with an API key passed in the Authorization\n      header. Most tenant-scoped endpoints additionally require a tenantId header.\n    applies_to: TrustLogix REST API (/api/*)\n    source: https://docs.trustlogix.io/trustlogix-api-documentation.md\n  - name: SessionLogin\n    type: http\n    scheme: custom\n    description: >-\n      POST /api/login exchanges loginId + password (+ optional TOTP for MFA) for a\n   \
  \   session; POST /api/logout ends it.\n    source: https://docs.trustlogix.io/trustlogix-api-documentation.md\n  - name: MCP-OAuth2\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      The TrustAI MCP Server authorizes agent connections with OAuth 2.0,\n      implementing RFC 9728 Protected Resource Metadata per the MCP Authentication\n      Specification. End-user OAuth tokens are propagated in the Authorization\n      header to carry end-user identity to the policy engine.\n    standards: [RFC9728]\n    source: https://docs.trustlogix.io/trust-ai/mcp-server.md\n  - name: SSO-OIDC\n    type: openIdConnect\n    description: >-\n      Console/tenant single sign-on via Azure Active Directory (MS Entra) and Okta,\n      with SCIM 2.0 user provisioning/deprovisioning and a regenerable SCIM token.\n    identity_providers: [Azure AD / MS Entra, Okta]\n    provisioning: SCIM 2.0\n    source: https://docs.trustlogix.io/integrations/single-sign-on.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustlogix/refs/heads/main/authentication/trustlogix-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Data Security
- Data Access Governance
- Data Security Posture Management
- Access Control
- Snowflake
- Databricks
- AI Security
- MCP
- Authorization
- Compliance
---
