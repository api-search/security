---
api_key_in: []
api_specs:
- filename: aifordatabase-chat-api-openapi.yml
  format: yaml
  label: AI for Database Chat API
  slug: aifordatabase-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-chat-api-openapi.yml
- filename: aifordatabase-connections-api-openapi.yml
  format: yaml
  label: AI for Database Connections API
  slug: aifordatabase-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-connections-api-openapi.yml
- filename: aifordatabase-conversations-api-openapi.yml
  format: yaml
  label: AI for Database Conversations API
  slug: aifordatabase-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-conversations-api-openapi.yml
- filename: aifordatabase-dashboards-api-openapi.yml
  format: yaml
  label: AI for Database Dashboards API
  slug: aifordatabase-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-dashboards-api-openapi.yml
- filename: aifordatabase-keys-api-openapi.yml
  format: yaml
  label: AI for Database Keys API
  slug: aifordatabase-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-keys-api-openapi.yml
- filename: aifordatabase-metrics-api-openapi.yml
  format: yaml
  label: AI for Database Metrics API
  slug: aifordatabase-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-metrics-api-openapi.yml
- filename: aifordatabase-query-approval-api-openapi.yml
  format: yaml
  label: AI for Database Query Approval API
  slug: aifordatabase-query-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-query-approval-api-openapi.yml
- filename: aifordatabase-saved-queries-api-openapi.yml
  format: yaml
  label: AI for Database Saved Queries API
  slug: aifordatabase-saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-saved-queries-api-openapi.yml
- filename: aifordatabase-usage-api-openapi.yml
  format: yaml
  label: AI for Database Usage API
  slug: aifordatabase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-usage-api-openapi.yml
- filename: aifordatabase-webhooks-api-openapi.yml
  format: yaml
  label: AI for Database Webhooks API
  slug: aifordatabase-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-webhooks-api-openapi.yml
- filename: aifordatabase-workflow-credentials-api-openapi.yml
  format: yaml
  label: AI for Database Workflow Credentials API
  slug: aifordatabase-workflow-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-workflow-credentials-api-openapi.yml
- filename: aifordatabase-workflows-api-openapi.yml
  format: yaml
  label: AI for Database Workflows API
  slug: aifordatabase-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aifordatabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI for Database secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AI for Database
provider_slug: aifordatabase
scheme_count: 1
schemes:
- applied: global
  applied_evidence: 'Document-level security: [{bearerAuth: []}] in the OpenAPI 3.1 spec — applied, not merely defined.'
  bearerFormat: API Key
  description: Platform API key starting with afd_
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aifordatabase-openapi.yml
  - https://www.aifordatabase.com/docs/authentication/
  type: http
  value_form: Bearer afd_...
slug: aifordatabase-authentication
source_filename: aifordatabase-authentication.yml
source_heading: Authentication Profile
source_url: https://www.aifordatabase.com/docs/authentication/
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.aifordatabase.com/docs/authentication/\nsources:\n- https://www.aifordatabase.com/docs/authentication/\n- https://aifordatabase.com/api/agents\n- openapi/aifordatabase-openapi.yml\napi: AI for Database API\nsummary:\n  types:\n  - http\n  model: scoped-bearer-api-key\n  oauth: false\n  openid_connect: false\n  mtls: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Platform API key starting with afd_\n  header: Authorization\n  value_form: 'Bearer afd_...'\n  applied: global\n  applied_evidence: 'Document-level security: [{bearerAuth: []}] in the OpenAPI 3.1 spec — applied, not merely defined.'\n  sources:\n  - openapi/aifordatabase-openapi.yml\n  - https://www.aifordatabase.com/docs/authentication/\nkey_management:\n  issue_ui: 'Settings > API Keys in app.aifordatabase.com'\n  issue_api: 'POST /api/v1/keys (createApiKey, admin scope)'\n  list_api: 'GET\
  \ /api/v1/keys (listApiKeys)'\n  revoke_api: 'DELETE /api/v1/keys/{id} (revokeApiKey)'\n  prefix: afd_\n  shown_once: true\n  expiry: optional per key\n  identity: 'A key authenticates on behalf of the organization, carrying the role of the user who created it.'\n  test_mode: false\n  test_mode_note: 'The provider states there are no afdb_live_ / afdb_test_ key variants.'\nscopes:\n  model: api-key-scopes\n  wildcard: '*'\n  docs: https://www.aifordatabase.com/docs/authentication/\n  note: >-\n    These are API-key permission scopes, not OAuth scopes — there is no authorization\n    server, no token endpoint and no /.well-known/oauth-authorization-server (404). No\n    OAuthScopes pointer is emitted for that reason; the scope reference lives here.\n  values:\n  - name: query\n    grants: Direct SQL execution, query submission, approval status, saved query runs\n  - name: chat\n    grants: Natural-language chat endpoints\n  - name: connections\n    grants: Sanitized database connection\
  \ metadata, schemas, and annotations\n  - name: dashboards\n    grants: Dashboards and widgets\n  - name: workflows\n    grants: Workflows and workflow runs\n  - name: workflow_credentials\n    grants: Encrypted outbound workflow credentials\n    additional_requirement: organization admin role\n  - name: usage\n    grants: Usage records and budget info\n  - name: webhooks\n    grants: Webhook endpoints and deliveries\n  - name: admin\n    grants: Key management and other admin operations\n  - name: '*'\n    grants: Full access\nrole_gate:\n  note: >-\n    Some operations require an organization admin role regardless of key scopes.\n    Workflow credential creation, rotation, listing and deletion require BOTH the\n    workflow_credentials scope AND the admin role.\nfailure_modes:\n- status: 401\n  code: UNAUTHORIZED\n  cause: Invalid or expired key\n- status: 403\n  code: FORBIDDEN\n  cause: Key lacks the required scope, or the operation additionally needs an admin role\nsecond_credential_class:\n\
  \  name: workflow credentials\n  purpose: 'Authenticate an outbound webhook action to ITS destination — not callers to this API.'\n  properties: [encrypted, write-only, destination-bound]\n  rule: 'Never accepted inline in a workflow definition; referenced by credentialId.'\n  operations: [createWorkflowCredential, rotateWorkflowCredential, deleteWorkflowCredential, listWorkflowCredentials, getWorkflowCredential]\n  docs: https://www.aifordatabase.com/docs/outbound-credentials/\nbest_practices_published:\n- Store API keys in environment variables, never in code.\n- Use the narrowest scopes necessary.\n- Rotate keys periodically and revoke unused keys.\n- Create separate keys per integration so each can be revoked independently.\nenterprise_sso:\n  saml2: true\n  oidc: true\n  mfa: 'available on all plans'\n  scope: 'Human sign-in to the product UI on the Enterprise plan; not an API authentication path.'\n  source: https://www.aifordatabase.com/trust/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/authentication/aifordatabase-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Database
- Analytics
- Developer Tools
- Natural Language Query
- Text-to-SQL
- Dashboards
- Business Intelligence
- Workflow Automation
- Alerts
- Agent-Native
- LLMSTxt
- OpenAPI
- Webhooks
- MCP
- PostgreSQL
- MySQL
- MongoDB
---
