---
api_key_in: []
api_specs:
- filename: cognition-labs-attachments-api-openapi.yml
  format: yaml
  label: Cognition Labs Attachments API
  slug: cognition-labs-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-attachments-api-openapi.yml
- filename: cognition-labs-consumption-api-openapi.yml
  format: yaml
  label: Cognition Labs Consumption API
  slug: cognition-labs-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-consumption-api-openapi.yml
- filename: cognition-labs-enterprise-v3-api-openapi.yml
  format: yaml
  label: Cognition Labs Enterprise (v3) API
  slug: cognition-labs-enterprise-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-enterprise-v3-api-openapi.yml
- filename: cognition-labs-knowledge-api-openapi.yml
  format: yaml
  label: Cognition Labs Knowledge API
  slug: cognition-labs-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-knowledge-api-openapi.yml
- filename: cognition-labs-messages-api-openapi.yml
  format: yaml
  label: Cognition Labs Messages API
  slug: cognition-labs-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-messages-api-openapi.yml
- filename: cognition-labs-organizations-v3-api-openapi.yml
  format: yaml
  label: Cognition Labs Organizations (v3) API
  slug: cognition-labs-organizations-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-organizations-v3-api-openapi.yml
- filename: cognition-labs-playbooks-api-openapi.yml
  format: yaml
  label: Cognition Labs Playbooks API
  slug: cognition-labs-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-playbooks-api-openapi.yml
- filename: cognition-labs-secrets-api-openapi.yml
  format: yaml
  label: Cognition Labs Secrets API
  slug: cognition-labs-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-secrets-api-openapi.yml
- filename: cognition-labs-sessions-api-openapi.yml
  format: yaml
  label: Cognition Labs Sessions API
  slug: cognition-labs-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-sessions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cognition Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognition Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cognition Labs
provider_slug: cognition-labs
scheme_count: 1
schemes:
- description: 'v1/v2 keys are prefixed apk_user_* (personal) or apk_* (service). The current v3 API uses service-user or personal access tokens prefixed cog_. Passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cognition-labs-openapi.yml
  type: http
slug: cognition-labs-authentication
source_filename: cognition-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognition-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'v1/v2 keys are prefixed apk_user_* (personal) or apk_* (service). The current\n    v3 API uses service-user or personal access tokens prefixed cog_. Passed as `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/cognition-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/authentication/cognition-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- AI Agent
- Autonomous Coding
- Software Engineering
- LLM
- Devin
---
