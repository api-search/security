---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mirascope-openapi-generated.yml
  format: yaml
  label: Mirascope API
  slug: mirascope-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirascope/refs/heads/main/openapi/_ae-authored/mirascope-openapi-generated.yml
auth_types: []
description: Authentication is performed via API keys set as environment variables for each LLM provider.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Mirascope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mirascope declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Mirascope
provider_slug: mirascope
scheme_count: 4
schemes:
- evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'
  how_to_obtain: Set the `ANTHROPIC_API_KEY` environment variable with your Anthropic API key.
  location: environment variable
  name: Anthropic
  type: apiKey
- evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'
  how_to_obtain: Set the `GOOGLE_API_KEY` environment variable with your Google API key.
  location: environment variable
  name: Google
  type: apiKey
- evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'
  how_to_obtain: Set the `OPENAI_API_KEY` environment variable with your OpenAI API key.
  location: environment variable
  name: OpenAI
  type: apiKey
- evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'
  how_to_obtain: Set the `TOGETHER_API_KEY` environment variable with your Together API key.
  location: environment variable
  name: Together
  type: apiKey
slug: mirascope-authentication
source_filename: mirascope-authentication.yml
source_heading: Authentication Profile
source_url: https://mirascope.com/docs/quickstart
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mirascope.com/docs/quickstart\nsources:\n- https://mirascope.com/docs/quickstart\n- https://mirascope.com/docs/v1/docs/getting-started/why\n- https://mirascope.com/docs/v1/docs/getting-started/help\n- https://mirascope.com/docs/v1/docs/getting-started/contributing\ndescription: Authentication is performed via API keys set as environment variables for each LLM provider.\nschemes:\n- type: apiKey\n  name: Anthropic\n  evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'\n  location: environment variable\n  how_to_obtain: Set the `ANTHROPIC_API_KEY` environment variable with your Anthropic API key.\n- type: apiKey\n  name: Google\n  evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'\n  location: environment variable\n  how_to_obtain: Set the `GOOGLE_API_KEY` environment\
  \ variable with your Google API key.\n- type: apiKey\n  name: OpenAI\n  evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'\n  location: environment variable\n  how_to_obtain: Set the `OPENAI_API_KEY` environment variable with your OpenAI API key.\n- type: apiKey\n  name: Together\n  evidence: 'To run any of the LLM-powered examples, you''ll need to set up API keys for your chosen provider:'\n  location: environment variable\n  how_to_obtain: Set the `TOGETHER_API_KEY` environment variable with your Together API key.\ndocs: https://mirascope.com/docs/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirascope/refs/heads/main/authentication/mirascope-authentication.yml
summary_line: 4 schemes
tags:
- LLM
- Framework
- AI
- Versioning
- Tracing
- Cost Tracking
---
