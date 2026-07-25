---
api_key_in: []
api_specs:
- filename: cognition-attachments-api-openapi.yml
  format: yaml
  label: Cognition AI Attachments API
  slug: cognition-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-attachments-api-openapi.yml
- filename: cognition-auditlogs-api-openapi.yml
  format: yaml
  label: Cognition AI AuditLogs API
  slug: cognition-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-auditlogs-api-openapi.yml
- filename: cognition-enterprise-api-openapi.yml
  format: yaml
  label: Cognition AI Enterprise API
  slug: cognition-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-enterprise-api-openapi.yml
- filename: cognition-knowledge-api-openapi.yml
  format: yaml
  label: Cognition AI Knowledge API
  slug: cognition-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-knowledge-api-openapi.yml
- filename: cognition-playbooks-api-openapi.yml
  format: yaml
  label: Cognition AI Playbooks API
  slug: cognition-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-playbooks-api-openapi.yml
- filename: cognition-secrets-api-openapi.yml
  format: yaml
  label: Cognition AI Secrets API
  slug: cognition-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-secrets-api-openapi.yml
- filename: cognition-sessions-api-openapi.yml
  format: yaml
  label: Cognition AI Sessions API
  slug: cognition-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-sessions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cognition Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognition AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cognition AI
provider_slug: cognition
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cognition-openapi.yml
  type: http
slug: cognition-authentication
source_filename: cognition-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognition-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cognition-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/authentication/cognition-authentication.yml
summary_line: http · 1 scheme
tags:
- Autonomous Agents
- AI Software Engineer
- Coding Agents
- Developer Productivity
- DevOps
- Code Migration
- Code Review
- GitHub Integration
- Enterprise AI
- Agentic Workflows
- IDE
- LLM Applications
---
