---
api_key_in:
- header
api_specs:
- filename: anthropic-messages-api-openapi.yml
  format: yaml
  label: Anthropic Messages API
  slug: anthropic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-messages-api-openapi.yml
- filename: anthropic-models-api-openapi.yml
  format: yaml
  label: Anthropic Models API
  slug: anthropic-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-models-api-openapi.yml
- filename: anthropic-message-batches-api-openapi.yml
  format: yaml
  label: Anthropic Message Batches API
  slug: anthropic-message-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-message-batches-api-openapi.yml
- filename: anthropic-files-api-openapi.yml
  format: yaml
  label: Anthropic Files API
  slug: anthropic-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-files-api-openapi.yml
- filename: anthropic-admin-api-openapi.yml
  format: yaml
  label: Anthropic Admin API
  slug: anthropic-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-admin-api-openapi.yml
- filename: anthropic-prompts-api-openapi.yml
  format: yaml
  label: Anthropic Prompts API
  slug: anthropic-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-prompts-api-openapi.yml
- filename: anthropic-token-counting-api-openapi.yml
  format: yaml
  label: Anthropic Token Counting API
  slug: anthropic-token-counting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-token-counting-api-openapi.yml
- filename: anthropic-skills-api-openapi.yml
  format: yaml
  label: Anthropic Skills API
  slug: anthropic-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-skills-api-openapi.yml
- filename: anthropic-usage-cost-api-openapi.yml
  format: yaml
  label: Anthropic Usage and Cost API
  slug: anthropic-usage-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-usage-cost-api-openapi.yml
- filename: anthropic-claude-code-analytics-api-openapi.yml
  format: yaml
  label: Anthropic Claude Code Analytics API
  slug: anthropic-claude-code-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-claude-code-analytics-api-openapi.yml
- filename: anthropic-managed-agents-api-openapi.yml
  format: yaml
  label: Anthropic Managed Agents API
  slug: anthropic-managed-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-managed-agents-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Anthropic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anthropic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anthropic
provider_slug: anthropic
scheme_count: 1
schemes:
- description: Your Admin API key for authentication (starts with sk-ant-admin...).
  in: header
  name: AdminApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/anthropic-admin-api-openapi.yml
  - openapi/anthropic-claude-code-analytics-api-openapi.yml
  - openapi/anthropic-files-api-openapi.yml
  - openapi/anthropic-managed-agents-api-openapi.yml
  - openapi/anthropic-message-batches-api-openapi.yml
  - openapi/anthropic-messages-api-openapi.yml
  - openapi/anthropic-models-api-openapi.yml
  - openapi/anthropic-prompts-api-openapi.yml
  - openapi/anthropic-skills-api-openapi.yml
  - openapi/anthropic-token-counting-api-openapi.yml
  - openapi/anthropic-usage-cost-api-openapi.yml
  type: apiKey
slug: anthropic-authentication
source_filename: anthropic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\ndocs: https://docs.anthropic.com/en/manage-claude/authentication\nsource: openapi/anthropic-admin-api-openapi.yml, openapi/anthropic-claude-code-analytics-api-openapi.yml,\n  openapi/anthropic-files-api-openapi.yml, openapi/anthropic-managed-agents-api-openapi.yml,\n  openapi/anthropic-message-batches-api-openapi.yml, openapi/anthropic-messages-api-openapi.yml,\n  openapi/anthropic-models-api-openapi.yml, openapi/anthropic-prompts-api-openapi.yml, openapi/anthropic-skills-api-openapi.yml,\n  openapi/anthropic-token-counting-api-openapi.yml, openapi/anthropic-usage-cost-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  additional_mechanisms:\n  - name: Admin API key\n    description: Privileged key (sk-ant-admin...) required for the Admin, Usage/Cost,\n      and Claude Code Analytics APIs, sent as x-api-key.\n  - name: Workload Identity Federation (WIF)\n    description: GA. Exchange short-lived OIDC tokens\
  \ from an external IdP (AWS IAM,\n      GCP, GitHub Actions, Kubernetes, Microsoft Entra ID, Okta, SPIFFE) for API access\n      instead of long-lived keys; SDKs handle token exchange and refresh.\n    docs: https://docs.anthropic.com/en/manage-claude/workload-identity-federation\n  - name: AWS SigV4\n    description: On Claude Platform on AWS, requests authenticate with AWS credentials\n      and SigV4 signatures via native AWS endpoints.\n  - name: MCP OAuth\n    description: Remote MCP servers and Managed Agents vault credentials use OAuth 2.0\n      (mcp_oauth), separate from the REST API key auth.\n  key_expiration: API keys and Admin API keys support optional expiration (expires_at)\n    configurable in the Claude Console.\nschemes:\n- name: AdminApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your Admin API key for authentication (starts with sk-ant-admin...).\n  sources:\n  - openapi/anthropic-admin-api-openapi.yml\n  - openapi/anthropic-claude-code-analytics-api-openapi.yml\n\
  \  - openapi/anthropic-files-api-openapi.yml\n  - openapi/anthropic-managed-agents-api-openapi.yml\n  - openapi/anthropic-message-batches-api-openapi.yml\n  - openapi/anthropic-messages-api-openapi.yml\n  - openapi/anthropic-models-api-openapi.yml\n  - openapi/anthropic-prompts-api-openapi.yml\n  - openapi/anthropic-skills-api-openapi.yml\n  - openapi/anthropic-token-counting-api-openapi.yml\n  - openapi/anthropic-usage-cost-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/authentication/anthropic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Claude
- Foundation Models
- Large Language Models
- Machine Learning
- MCP
- Agents
---
