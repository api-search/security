---
api_key_in:
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Expected Parrot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Expected Parrot secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Expected Parrot
provider_slug: expected-parrot
scheme_count: 2
schemes:
- description: Personal Expected Parrot key from the account page; grants access to all available models via the Expected Parrot server (remote inference) and to posting/sharing content on the platform. Stored via the account, a local file, or an environment variable.
  in: environment
  managed_at: https://www.expectedparrot.com/home/keys
  name: ExpectedParrotApiKey
  parameter: EXPECTED_PARROT_API_KEY
  type: apiKey
- description: Optional user-supplied keys for model providers (Anthropic, Azure, Bedrock, Deep Infra, DeepSeek, Google, Groq, Mistral, OpenAI, Perplexity, Together, Xai) for local inference without the Expected Parrot server.
  in: environment
  name: ProviderModelKeys
  type: apiKey
slug: expected-parrot-authentication
source_filename: expected-parrot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.expectedparrot.com/en/latest/api_keys.md\ndocs: https://docs.expectedparrot.com/en/latest/api_keys.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - environment\n  notes: Expected Parrot uses an API-key model rather than OAuth. An Expected Parrot\n    API key (EXPECTED_PARROT_API_KEY) authenticates remote inference and platform\n    (Coop) storage/sharing; alternatively users supply their own third-party model\n    provider keys for local inference. No OAuth2 or OIDC surface is published.\nschemes:\n- name: ExpectedParrotApiKey\n  type: apiKey\n  in: environment\n  parameter: EXPECTED_PARROT_API_KEY\n  description: Personal Expected Parrot key from the account page; grants access to\n    all available models via the Expected Parrot server (remote inference) and to\n    posting/sharing content on the platform. Stored via the account, a local file,\n    or an environment variable.\n  managed_at: https://www.expectedparrot.com/home/keys\n\
  - name: ProviderModelKeys\n  type: apiKey\n  in: environment\n  description: Optional user-supplied keys for model providers (Anthropic, Azure, Bedrock,\n    Deep Infra, DeepSeek, Google, Groq, Mistral, OpenAI, Perplexity, Together, Xai)\n    for local inference without the Expected Parrot server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expected-parrot/refs/heads/main/authentication/expected-parrot-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Surveys
- Research
- Social Science
- Synthetic Data
- AI Agents
- Market Research
- Python
---
