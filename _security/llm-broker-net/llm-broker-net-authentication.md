---
anonymous_access: false
api_key_in: []
api_specs:
- filename: llm-broker-net-account-api-openapi.yml
  format: yaml
  label: LLM Broker Account API
  slug: llm-broker-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-account-api-openapi.yml
- filename: llm-broker-net-account-payment-api-openapi.yml
  format: yaml
  label: LLM Broker Account & payment API
  slug: llm-broker-net-account-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-account-payment-api-openapi.yml
- filename: llm-broker-net-chat-api-openapi.yml
  format: yaml
  label: LLM Broker Chat API
  slug: llm-broker-net-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-chat-api-openapi.yml
- filename: llm-broker-net-models-api-openapi.yml
  format: yaml
  label: LLM Broker Models API
  slug: llm-broker-net-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-models-api-openapi.yml
- filename: llm-broker-net-openai-compatible-api-openapi.yml
  format: yaml
  label: LLM Broker Open AI Compatible API
  slug: llm-broker-net-openai-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-openai-compatible-api-openapi.yml
- filename: llm-broker-net-routing-api-openapi.yml
  format: yaml
  label: LLM Broker Routing API
  slug: llm-broker-net-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-routing-api-openapi.yml
- filename: llm-broker-net-status-api-openapi.yml
  format: yaml
  label: LLM Broker Status API
  slug: llm-broker-net-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-status-api-openapi.yml
- filename: llm-broker-net-video-api-openapi.yml
  format: yaml
  label: LLM Broker Video API
  slug: llm-broker-net-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llm-broker-net/openapi/llm-broker-net-video-api-openapi.yml
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LLM Broker Authentication
name_suffix: Authentication
oauth_flows: []
overview: LLM Broker declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LLM Broker
provider_slug: llm-broker-net
scheme_count: 1
schemes:
- evidence: 'curl -s https://api.llm-broker.net/api/v1/chat/completions \ -H "Authorization: Bearer ast_try" \'
  header: Authorization
  how_to_obtain: Obtain an API key by creating an account (POST /api/v1/broker/accounts) and receiving a key such as ast_sk_…
  location: header
  name: Bearer
  type: http-bearer
slug: llm-broker-net-authentication
source_filename: llm-broker-net-authentication.yml
source_heading: Authentication Profile
source_url: https://llm-broker.net/quickstart
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://llm-broker.net/quickstart\nsources:\n- https://llm-broker.net/quickstart\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -s https://api.llm-broker.net/api/v1/chat/completions \\ -H \"Authorization: Bearer ast_try\" \\'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API key by creating an account (POST /api/v1/broker/accounts) and receiving a key such as ast_sk_…\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://llm-broker.net/quickstart\n"
source_yaml_url: https://artifacts.apis.io/llm-broker-net/authentication/llm-broker-net-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
