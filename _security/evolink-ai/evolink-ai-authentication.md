---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evolink-ai-openapi-generated.yml
  format: yaml
  label: EvoLink API
  slug: evolink-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evolink-ai/openapi/_ae-authored/evolink-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for EvoLink APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EvoLink Authentication
name_suffix: Authentication
oauth_flows: []
overview: EvoLink declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EvoLink
provider_slug: evolink-ai
scheme_count: 1
schemes:
- evidence: '##All APIs require Bearer Token authentication##'
  header: Authorization
  how_to_obtain: 'Get API Key: Visit API Key Management Page to get your API Key'
  location: header
  name: Bearer Token
  type: http-bearer
slug: evolink-ai-authentication
source_filename: evolink-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://evolink.ai/signup?returnUrl=/dashboard/keys&utm_source=llms_txt
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://evolink.ai/signup?returnUrl=/dashboard/keys&utm_source=llms_txt\nsources:\n- https://evolink.ai/signup?returnUrl=/dashboard/keys&utm_source=llms_txt\n- https://evolink.ai/docs/en/api-manual/language-series/kimi/chat-completions/chat-completions-quickstart\n- https://evolink.ai/docs/en/cli/setup\n- https://evolink.ai/docs/en/mcp/other-clients#local-mcp\ndescription: Authentication methods for EvoLink APIs\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: '##All APIs require Bearer Token authentication##'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Get API Key: Visit API Key Management Page to get your API Key'\ndocs: https://evolink.ai/signup?returnUrl=/dashboard/keys&utm_source=llms_txt\n"
source_yaml_url: https://artifacts.apis.io/evolink-ai/authentication/evolink-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI Model API
- Production AI
- Unified API
- Multi‑Model Access
- Video Generation
- Image Generation
- Audio Generation
- LLM
---
