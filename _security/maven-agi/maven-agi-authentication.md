---
api_key_in: []
api_specs:
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Conversation API
  slug: maven-agi-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Knowledge API
  slug: maven-agi-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Actions API
  slug: maven-agi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Users API
  slug: maven-agi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Agents API
  slug: maven-agi-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Events API
  slug: maven-agi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Triggers API
  slug: maven-agi-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI App Settings API
  slug: maven-agi-app-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
- filename: maven-agi-openapi.yml
  format: yaml
  label: Maven AGI Analytics API
  slug: maven-agi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/openapi/maven-agi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maven Agi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maven AGI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maven AGI
provider_slug: maven-agi
scheme_count: 1
schemes:
- description: HTTP Basic authentication using the App ID as the username and the App Secret as the password. Requests must also send X-Organization-Id and X-Agent-Id headers to scope the call to an organization and agent.
  name: appAuth
  scheme: basic
  sources:
  - openapi/maven-agi-openapi.yml
  type: http
slug: maven-agi-authentication
source_filename: maven-agi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maven-agi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: appAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the App ID as the username and the App Secret\n    as the password. Requests must also send X-Organization-Id and X-Agent-Id headers to scope\n    the call to an organization and agent.\n  sources:\n  - openapi/maven-agi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven-agi/refs/heads/main/authentication/maven-agi-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- Customer Support
- Customer Experience
- Conversational AI
- Knowledge
---
