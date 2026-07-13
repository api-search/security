---
api_key_in: []
api_specs:
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Sessions API
  slug: devin-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Messages API
  slug: devin-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Attachments API
  slug: devin-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Knowledge API
  slug: devin-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Playbooks API
  slug: devin-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Secrets API
  slug: devin-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Organizations API
  slug: devin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Enterprise API
  slug: devin-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Usage & Consumption API
  slug: devin-usage-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
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
- description: 'v1/v2 keys are prefixed apk_user_* (personal) or apk_* (service). The current v3 API uses service-user or personal access tokens prefixed cog_. Passed as `Authorization: Bearer YOUR_API_KEY`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cognition-labs-openapi.yml
  type: http
slug: cognition-labs-authentication
source_filename: cognition-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognition-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'v1/v2 keys are prefixed apk_user_* (personal) or apk_* (service). The current\n    v3 API uses service-user or personal access tokens prefixed cog_. Passed as `Authorization:\n    Bearer YOUR_API_KEY`.'\n  sources:\n  - openapi/cognition-labs-openapi.yml\n"
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
