---
api_key_in: []
api_specs:
- filename: pydantic-ai-discovery-openapi.yml
  format: yaml
  label: PydanticAI Agent Framework
  slug: pydantic-ai-agent-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-discovery-openapi.yml
- filename: pydantic-ai-logfire-openapi.yml
  format: yaml
  label: Pydantic Logfire
  slug: pydantic-logfire
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-logfire-openapi.yml
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
- AI
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
