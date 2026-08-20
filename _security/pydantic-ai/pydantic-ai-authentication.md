---
api_key_in: []
api_specs:
- filename: pydantic-ai-alerts-api-openapi.yml
  format: yaml
  label: PydanticAI Alerts API
  slug: pydantic-ai-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-alerts-api-openapi.yml
- filename: pydantic-ai-api-keys-api-openapi.yml
  format: yaml
  label: PydanticAI API Keys API
  slug: pydantic-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-api-keys-api-openapi.yml
- filename: pydantic-ai-audit-logs-api-openapi.yml
  format: yaml
  label: PydanticAI Audit Logs API
  slug: pydantic-ai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-audit-logs-api-openapi.yml
- filename: pydantic-ai-billing-api-openapi.yml
  format: yaml
  label: PydanticAI Billing API
  slug: pydantic-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-billing-api-openapi.yml
- filename: pydantic-ai-channels-api-openapi.yml
  format: yaml
  label: PydanticAI Channels API
  slug: pydantic-ai-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-channels-api-openapi.yml
- filename: pydantic-ai-dashboards-api-openapi.yml
  format: yaml
  label: PydanticAI Dashboards API
  slug: pydantic-ai-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-dashboards-api-openapi.yml
- filename: pydantic-ai-discovery-api-openapi.yml
  format: yaml
  label: PydanticAI discovery API
  slug: pydantic-ai-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-discovery-api-openapi.yml
- filename: pydantic-ai-group-mappings-api-openapi.yml
  format: yaml
  label: PydanticAI Group Mappings API
  slug: pydantic-ai-group-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-group-mappings-api-openapi.yml
- filename: pydantic-ai-instance-api-openapi.yml
  format: yaml
  label: PydanticAI Instance API
  slug: pydantic-ai-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-instance-api-openapi.yml
- filename: pydantic-ai-invitations-api-openapi.yml
  format: yaml
  label: PydanticAI Invitations API
  slug: pydantic-ai-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-invitations-api-openapi.yml
- filename: pydantic-ai-members-api-openapi.yml
  format: yaml
  label: PydanticAI Members API
  slug: pydantic-ai-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-members-api-openapi.yml
- filename: pydantic-ai-oauth-api-openapi.yml
  format: yaml
  label: PydanticAI OAuth API
  slug: pydantic-ai-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-oauth-api-openapi.yml
- filename: pydantic-ai-organizations-api-openapi.yml
  format: yaml
  label: PydanticAI Organizations API
  slug: pydantic-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-organizations-api-openapi.yml
- filename: pydantic-ai-projects-api-openapi.yml
  format: yaml
  label: PydanticAI Projects API
  slug: pydantic-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-projects-api-openapi.yml
- filename: pydantic-ai-scim-api-openapi.yml
  format: yaml
  label: PydanticAI SCIM API
  slug: pydantic-ai-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-scim-api-openapi.yml
- filename: pydantic-ai-usage-api-openapi.yml
  format: yaml
  label: PydanticAI Usage API
  slug: pydantic-ai-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-usage-api-openapi.yml
- filename: pydantic-ai-variables-api-openapi.yml
  format: yaml
  label: PydanticAI Variables API
  slug: pydantic-ai-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-variables-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pydantic Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PydanticAI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PydanticAI
provider_slug: pydantic-ai
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: api/oauth/authorize
    flow: authorizationCode
    scopes: 38
    tokenUrl: /api/oauth/token
  name: OAuth2AuthorizationCodeBearer
  sources:
  - openapi/pydantic-ai-logfire-openapi.yml
  type: oauth2
slug: pydantic-ai-authentication
source_filename: pydantic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pydantic-ai-logfire-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2AuthorizationCodeBearer\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: api/oauth/authorize\n    tokenUrl: /api/oauth/token\n    scopes: 38\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/authentication/pydantic-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Python
- LLM
- Type Safety
- Structured Outputs
- Dependency Injection
- OpenAI
- Anthropic
- Gemini
- Observability
- Framework
---
