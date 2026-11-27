---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bookmyhost-public-openapi.json
  format: json
  label: BookMyHost API
  slug: bookmyhost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bookmyhost/openapi/_original/bookmyhost-public-openapi.json
- filename: openapi.json
  format: json
  label: BookMyHost AI API (LiteLLM proxy)
  slug: bookmyhost-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bookmyhost/openapi/_original/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Blazing Bullet Private Limited Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blazing Bullet Private Limited secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blazing Bullet Private Limited
provider_slug: bookmyhost
scheme_count: 1
schemes:
- description: Bearer token
  in: header
  name: APIKeyHeader
  parameter: x-litellm-api-key
  sources:
  - openapi/bookmyhost-a2a-api-openapi.yml
  - openapi/bookmyhost-a2a-registration-api-openapi.yml
  - openapi/bookmyhost-access-groups-api-openapi.yml
  - openapi/bookmyhost-adaptive-router-api-openapi.yml
  - openapi/bookmyhost-agent-management-api-openapi.yml
  - openapi/bookmyhost-agents-api-openapi.yml
  - openapi/bookmyhost-anthropic-pass-through-api-openapi.yml
  - openapi/bookmyhost-anthropic-passthrough-api-openapi.yml
  - openapi/bookmyhost-anthropic-skills-api-openapi.yml
  - openapi/bookmyhost-assemblyai-eu-pass-through-api-openapi.yml
  - openapi/bookmyhost-assemblyai-pass-through-api-openapi.yml
  - openapi/bookmyhost-assistants-api-openapi.yml
  - openapi/bookmyhost-audio-api-openapi.yml
  - openapi/bookmyhost-audit-logging-api-openapi.yml
  - openapi/bookmyhost-azure-ai-pass-through-api-openapi.yml
  - openapi/bookmyhost-azure-pass-through-api-openapi.yml
  - openapi/bookmyhost-batch-api-openapi.yml
  - openapi/bookmyhost-bedrock-pass-through-api-openapi.yml
  - openapi/bookmyhost-beta-a2a-agents-api-openapi.yml
  - openapi/bookmyhost-beta-agents-api-openapi.yml
  - openapi/bookmyhost-beta-mcp-api-openapi.yml
  - openapi/bookmyhost-budget-management-api-openapi.yml
  - openapi/bookmyhost-budget-spend-tracking-api-openapi.yml
  - openapi/bookmyhost-cache-settings-api-openapi.yml
  - openapi/bookmyhost-caching-api-openapi.yml
  - openapi/bookmyhost-chat-completions-api-openapi.yml
  - openapi/bookmyhost-claude-code-marketplace-api-openapi.yml
  - openapi/bookmyhost-cohere-pass-through-api-openapi.yml
  - openapi/bookmyhost-completions-api-openapi.yml
  - openapi/bookmyhost-compliance-api-openapi.yml
  - openapi/bookmyhost-config-api-openapi.yml
  - openapi/bookmyhost-containers-api-openapi.yml
  - openapi/bookmyhost-coordination-redis-settings-api-openapi.yml
  - openapi/bookmyhost-cost-tracking-api-openapi.yml
  - openapi/bookmyhost-credential-management-api-openapi.yml
  - openapi/bookmyhost-cursor-pass-through-api-openapi.yml
  - openapi/bookmyhost-customer-management-api-openapi.yml
  - openapi/bookmyhost-debug-api-openapi.yml
  - openapi/bookmyhost-email-management-api-openapi.yml
  - openapi/bookmyhost-embeddings-api-openapi.yml
  - openapi/bookmyhost-evals-api-openapi.yml
  - openapi/bookmyhost-experimental-api-openapi.yml
  - openapi/bookmyhost-fallback-management-api-openapi.yml
  - openapi/bookmyhost-files-api-openapi.yml
  - openapi/bookmyhost-fine-tuning-api-openapi.yml
  - openapi/bookmyhost-gemini-agents-api-openapi.yml
  - openapi/bookmyhost-google-ai-studio-pass-through-api-openapi.yml
  - openapi/bookmyhost-google-genai-endpoints-api-openapi.yml
  - openapi/bookmyhost-guardrails-api-openapi.yml
  - openapi/bookmyhost-health-api-openapi.yml
  - openapi/bookmyhost-images-api-openapi.yml
  - openapi/bookmyhost-interactions-api-openapi.yml
  - openapi/bookmyhost-internal-user-management-api-openapi.yml
  - openapi/bookmyhost-jwt-mappings-api-openapi.yml
  - openapi/bookmyhost-key-management-api-openapi.yml
  - openapi/bookmyhost-langfuse-passthrough-api-openapi.yml
  - openapi/bookmyhost-litellm-api-api-openapi.yml
  - openapi/bookmyhost-litellm-api-openapi.yml
  - openapi/bookmyhost-llm-utils-api-openapi.yml
  - openapi/bookmyhost-logging-callbacks-api-openapi.yml
  - openapi/bookmyhost-mcp-api-openapi.yml
  - openapi/bookmyhost-mcp-rest-api-openapi.yml
  - openapi/bookmyhost-memory-management-api-openapi.yml
  - openapi/bookmyhost-milvus-pass-through-api-openapi.yml
  - openapi/bookmyhost-mistral-pass-through-api-openapi.yml
  - openapi/bookmyhost-model-management-api-openapi.yml
  - openapi/bookmyhost-moderations-api-openapi.yml
  - openapi/bookmyhost-ocr-api-openapi.yml
  - openapi/bookmyhost-openai-pass-through-api-openapi.yml
  - openapi/bookmyhost-organization-management-api-openapi.yml
  - openapi/bookmyhost-passthrough-api-openapi.yml
  - openapi/bookmyhost-plugins-api-openapi.yml
  - openapi/bookmyhost-policies-api-openapi.yml
  - openapi/bookmyhost-policy-engine-api-openapi.yml
  - openapi/bookmyhost-project-management-api-openapi.yml
  - openapi/bookmyhost-prompts-api-openapi.yml
  - openapi/bookmyhost-provider-api-openapi.yml
  - openapi/bookmyhost-providers-api-openapi.yml
  - openapi/bookmyhost-public-api-openapi.yml
  - openapi/bookmyhost-rag-api-openapi.yml
  - openapi/bookmyhost-realtime-api-openapi.yml
  - openapi/bookmyhost-rerank-api-openapi.yml
  - openapi/bookmyhost-responses-api-openapi.yml
  - openapi/bookmyhost-robots-txt-api-openapi.yml
  - openapi/bookmyhost-router-settings-api-openapi.yml
  - openapi/bookmyhost-routes-api-openapi.yml
  - openapi/bookmyhost-rust-control-plane-api-openapi.yml
  - openapi/bookmyhost-scim-api-openapi.yml
  - openapi/bookmyhost-search-api-openapi.yml
  - openapi/bookmyhost-search-tools-api-openapi.yml
  - openapi/bookmyhost-settings-api-openapi.yml
  - openapi/bookmyhost-sso-settings-api-openapi.yml
  - openapi/bookmyhost-tag-management-api-openapi.yml
  - openapi/bookmyhost-team-api-openapi.yml
  - openapi/bookmyhost-team-management-api-openapi.yml
  - openapi/bookmyhost-tools-api-openapi.yml
  - openapi/bookmyhost-toolset-api-openapi.yml
  - openapi/bookmyhost-ui-settings-api-openapi.yml
  - openapi/bookmyhost-ui-theme-settings-api-openapi.yml
  - openapi/bookmyhost-usage-ai-api-openapi.yml
  - openapi/bookmyhost-user-agent-analytics-api-openapi.yml
  - openapi/bookmyhost-vector-store-management-api-openapi.yml
  - openapi/bookmyhost-vector-stores-api-openapi.yml
  - openapi/bookmyhost-vertex-ai-pass-through-api-openapi.yml
  - openapi/bookmyhost-videos-api-openapi.yml
  - openapi/bookmyhost-vllm-pass-through-api-openapi.yml
  - openapi/bookmyhost-watsonx-pass-through-api-openapi.yml
  - openapi/bookmyhost-websocket-api-openapi.yml
  - openapi/bookmyhost-well-known-api-openapi.yml
  - openapi/bookmyhost-workflow-management-api-openapi.yml
  type: apiKey
slug: bookmyhost-authentication
source_filename: bookmyhost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/bookmyhost-a2a-api-openapi.yml, openapi/bookmyhost-a2a-registration-api-openapi.yml,\n  openapi/bookmyhost-access-groups-api-openapi.yml, openapi/bookmyhost-adaptive-router-api-openapi.yml,\n  openapi/bookmyhost-agent-management-api-openapi.yml, openapi/bookmyhost-agents-api-openapi.yml,\n  openapi/bookmyhost-anthropic-pass-through-api-openapi.yml, openapi/bookmyhost-anthropic-passthrough-api-openapi.yml,\n  openapi/bookmyhost-anthropic-skills-api-openapi.yml, openapi/bookmyhost-assemblyai-eu-pass-through-api-openapi.yml,\n  openapi/bookmyhost-assemblyai-pass-through-api-openapi.yml, openapi/bookmyhost-assistants-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-litellm-api-key\n  description: Bearer token\n  sources:\n  - openapi/bookmyhost-a2a-api-openapi.yml\n  - openapi/bookmyhost-a2a-registration-api-openapi.yml\n\
  \  - openapi/bookmyhost-access-groups-api-openapi.yml\n  - openapi/bookmyhost-adaptive-router-api-openapi.yml\n  - openapi/bookmyhost-agent-management-api-openapi.yml\n  - openapi/bookmyhost-agents-api-openapi.yml\n  - openapi/bookmyhost-anthropic-pass-through-api-openapi.yml\n  - openapi/bookmyhost-anthropic-passthrough-api-openapi.yml\n  - openapi/bookmyhost-anthropic-skills-api-openapi.yml\n  - openapi/bookmyhost-assemblyai-eu-pass-through-api-openapi.yml\n  - openapi/bookmyhost-assemblyai-pass-through-api-openapi.yml\n  - openapi/bookmyhost-assistants-api-openapi.yml\n  - openapi/bookmyhost-audio-api-openapi.yml\n  - openapi/bookmyhost-audit-logging-api-openapi.yml\n  - openapi/bookmyhost-azure-ai-pass-through-api-openapi.yml\n  - openapi/bookmyhost-azure-pass-through-api-openapi.yml\n  - openapi/bookmyhost-batch-api-openapi.yml\n  - openapi/bookmyhost-bedrock-pass-through-api-openapi.yml\n  - openapi/bookmyhost-beta-a2a-agents-api-openapi.yml\n  - openapi/bookmyhost-beta-agents-api-openapi.yml\n\
  \  - openapi/bookmyhost-beta-mcp-api-openapi.yml\n  - openapi/bookmyhost-budget-management-api-openapi.yml\n  - openapi/bookmyhost-budget-spend-tracking-api-openapi.yml\n  - openapi/bookmyhost-cache-settings-api-openapi.yml\n  - openapi/bookmyhost-caching-api-openapi.yml\n  - openapi/bookmyhost-chat-completions-api-openapi.yml\n  - openapi/bookmyhost-claude-code-marketplace-api-openapi.yml\n  - openapi/bookmyhost-cohere-pass-through-api-openapi.yml\n  - openapi/bookmyhost-completions-api-openapi.yml\n  - openapi/bookmyhost-compliance-api-openapi.yml\n  - openapi/bookmyhost-config-api-openapi.yml\n  - openapi/bookmyhost-containers-api-openapi.yml\n  - openapi/bookmyhost-coordination-redis-settings-api-openapi.yml\n  - openapi/bookmyhost-cost-tracking-api-openapi.yml\n  - openapi/bookmyhost-credential-management-api-openapi.yml\n  - openapi/bookmyhost-cursor-pass-through-api-openapi.yml\n  - openapi/bookmyhost-customer-management-api-openapi.yml\n  - openapi/bookmyhost-debug-api-openapi.yml\n\
  \  - openapi/bookmyhost-email-management-api-openapi.yml\n  - openapi/bookmyhost-embeddings-api-openapi.yml\n  - openapi/bookmyhost-evals-api-openapi.yml\n  - openapi/bookmyhost-experimental-api-openapi.yml\n  - openapi/bookmyhost-fallback-management-api-openapi.yml\n  - openapi/bookmyhost-files-api-openapi.yml\n  - openapi/bookmyhost-fine-tuning-api-openapi.yml\n  - openapi/bookmyhost-gemini-agents-api-openapi.yml\n  - openapi/bookmyhost-google-ai-studio-pass-through-api-openapi.yml\n  - openapi/bookmyhost-google-genai-endpoints-api-openapi.yml\n  - openapi/bookmyhost-guardrails-api-openapi.yml\n  - openapi/bookmyhost-health-api-openapi.yml\n  - openapi/bookmyhost-images-api-openapi.yml\n  - openapi/bookmyhost-interactions-api-openapi.yml\n  - openapi/bookmyhost-internal-user-management-api-openapi.yml\n  - openapi/bookmyhost-jwt-mappings-api-openapi.yml\n  - openapi/bookmyhost-key-management-api-openapi.yml\n  - openapi/bookmyhost-langfuse-passthrough-api-openapi.yml\n  - openapi/bookmyhost-litellm-api-api-openapi.yml\n\
  \  - openapi/bookmyhost-litellm-api-openapi.yml\n  - openapi/bookmyhost-llm-utils-api-openapi.yml\n  - openapi/bookmyhost-logging-callbacks-api-openapi.yml\n  - openapi/bookmyhost-mcp-api-openapi.yml\n  - openapi/bookmyhost-mcp-rest-api-openapi.yml\n  - openapi/bookmyhost-memory-management-api-openapi.yml\n  - openapi/bookmyhost-milvus-pass-through-api-openapi.yml\n  - openapi/bookmyhost-mistral-pass-through-api-openapi.yml\n  - openapi/bookmyhost-model-management-api-openapi.yml\n  - openapi/bookmyhost-moderations-api-openapi.yml\n  - openapi/bookmyhost-ocr-api-openapi.yml\n  - openapi/bookmyhost-openai-pass-through-api-openapi.yml\n  - openapi/bookmyhost-organization-management-api-openapi.yml\n  - openapi/bookmyhost-passthrough-api-openapi.yml\n  - openapi/bookmyhost-plugins-api-openapi.yml\n  - openapi/bookmyhost-policies-api-openapi.yml\n  - openapi/bookmyhost-policy-engine-api-openapi.yml\n  - openapi/bookmyhost-project-management-api-openapi.yml\n  - openapi/bookmyhost-prompts-api-openapi.yml\n\
  \  - openapi/bookmyhost-provider-api-openapi.yml\n  - openapi/bookmyhost-providers-api-openapi.yml\n  - openapi/bookmyhost-public-api-openapi.yml\n  - openapi/bookmyhost-rag-api-openapi.yml\n  - openapi/bookmyhost-realtime-api-openapi.yml\n  - openapi/bookmyhost-rerank-api-openapi.yml\n  - openapi/bookmyhost-responses-api-openapi.yml\n  - openapi/bookmyhost-robots-txt-api-openapi.yml\n  - openapi/bookmyhost-router-settings-api-openapi.yml\n  - openapi/bookmyhost-routes-api-openapi.yml\n  - openapi/bookmyhost-rust-control-plane-api-openapi.yml\n  - openapi/bookmyhost-scim-api-openapi.yml\n  - openapi/bookmyhost-search-api-openapi.yml\n  - openapi/bookmyhost-search-tools-api-openapi.yml\n  - openapi/bookmyhost-settings-api-openapi.yml\n  - openapi/bookmyhost-sso-settings-api-openapi.yml\n  - openapi/bookmyhost-tag-management-api-openapi.yml\n  - openapi/bookmyhost-team-api-openapi.yml\n  - openapi/bookmyhost-team-management-api-openapi.yml\n  - openapi/bookmyhost-tools-api-openapi.yml\n\
  \  - openapi/bookmyhost-toolset-api-openapi.yml\n  - openapi/bookmyhost-ui-settings-api-openapi.yml\n  - openapi/bookmyhost-ui-theme-settings-api-openapi.yml\n  - openapi/bookmyhost-usage-ai-api-openapi.yml\n  - openapi/bookmyhost-user-agent-analytics-api-openapi.yml\n  - openapi/bookmyhost-vector-store-management-api-openapi.yml\n  - openapi/bookmyhost-vector-stores-api-openapi.yml\n  - openapi/bookmyhost-vertex-ai-pass-through-api-openapi.yml\n  - openapi/bookmyhost-videos-api-openapi.yml\n  - openapi/bookmyhost-vllm-pass-through-api-openapi.yml\n  - openapi/bookmyhost-watsonx-pass-through-api-openapi.yml\n  - openapi/bookmyhost-websocket-api-openapi.yml\n  - openapi/bookmyhost-well-known-api-openapi.yml\n  - openapi/bookmyhost-workflow-management-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/bookmyhost/authentication/bookmyhost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cloud
- Hosting
- VPS
- India
---
