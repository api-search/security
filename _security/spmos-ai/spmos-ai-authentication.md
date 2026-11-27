---
anonymous_access: false
api_key_in: []
api_specs:
- filename: spmos-ai-health-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Health API
  slug: spmos-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-health-api-openapi.yml
- filename: spmos-ai-livez-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Livez API
  slug: spmos-ai-livez-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-livez-api-openapi.yml
- filename: spmos-ai-messages-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Messages API
  slug: spmos-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-messages-api-openapi.yml
- filename: spmos-ai-readyz-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Readyz API
  slug: spmos-ai-readyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-readyz-api-openapi.yml
- filename: spmos-ai-responses-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Responses API
  slug: spmos-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-responses-api-openapi.yml
- filename: spmos-ai-spm-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Spm API
  slug: spmos-ai-spm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-spm-api-openapi.yml
- filename: spmos-ai-well-known-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. .well Known API
  slug: spmos-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-well-known-api-openapi.yml
- filename: spmos-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Veridical Tech, Inc. Chat Completions API
  slug: spmos-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spmos-ai/openapi/spmos-ai-chat-completions-api-openapi.yml
auth_types: []
description: Authentication schemes for Veridical Tech, Inc. SPM APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Veridical Tech, Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veridical Tech, Inc. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Veridical Tech, Inc.
provider_slug: spmos-ai
scheme_count: 1
schemes:
- evidence: Anthropic-dialect clients may send the same key in x-api-key ; both headers are accepted.
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
slug: spmos-ai-authentication
source_filename: spmos-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.spmos.ai/authentication
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.spmos.ai/authentication\nsources:\n- https://docs.spmos.ai/authentication\n- https://docs.spmos.ai/quickstart\ndescription: Authentication schemes for Veridical Tech, Inc. SPM APIs\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Anthropic-dialect clients may send the same key in x-api-key ; both headers are accepted.\n  location: header\n  header: x-api-key\nnote: Both the Authorization Bearer header and the x-api-key header are accepted for the same API key. 1 extracted row(s) were dropped because\n  their quote was not on the page.\ndocs: https://docs.spmos.ai/authentication\n"
source_yaml_url: https://artifacts.apis.io/spmos-ai/authentication/spmos-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Memory
- Governance
- Enterprise
- Long-Term
---
