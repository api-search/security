---
api_key_in: []
api_specs:
- filename: stacks-ai-openapi-original.yml
  format: yaml
  label: StackAI API
  slug: stackai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Stacks Ai Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Stacks Ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Stacks Ai
provider_slug: stacks-ai
scheme_count: 2
schemes:
- applies_to:
  - Knowledge Bases
  - Document upload
  - Run deployed flow
  description: 'Bearer API key (organization / personal token) in the Authorization header, e.g. `Authorization: Bearer <YOUR_API_KEY>`. Generated in Settings -> API Keys.'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/stacks-ai-openapi-original.yml
  type: http
- applies_to:
  - Run deployed flow
  - Analytics
  description: Authorization header. OAuth2 password-grant token scheme (no scopes declared).
  flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/stacks-ai-openapi-original.yml
  type: oauth2
slug: stacks-ai-authentication
source_filename: stacks-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stacks-ai-openapi-original.yml\ndocs: https://docs.stackai.com/interface-and-deployment/end-user-interfaces/api\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\n  notes: >-\n    Deployed-flow and document-upload endpoints authenticate with a Bearer public API key (the\n    organization token), passed in the Authorization header. API keys are generated in the StackAI\n    console under Settings -> API Keys and can be personal or organization scoped. Some management and\n    analytics endpoints declare an OAuth2 password-grant token scheme (tokenUrl \"token\"). No scopes are\n    defined on the OAuth2 flow.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer API key (organization / personal token) in the Authorization header, e.g.\n    `Authorization: Bearer <YOUR_API_KEY>`. Generated in Settings -> API Keys.\n  applies_to:\n  - Knowledge Bases\n  - Document\
  \ upload\n  - Run deployed flow\n  sources:\n  - openapi/stacks-ai-openapi-original.yml\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  description: Authorization header. OAuth2 password-grant token scheme (no scopes declared).\n  applies_to:\n  - Run deployed flow\n  - Analytics\n  sources:\n  - openapi/stacks-ai-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/authentication/stacks-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- AI
- Agents
- Artificial Intelligence
- LLM
- No-Code
- Automation
- Workflows
- RAG
- Knowledge Base
- Enterprise
---
