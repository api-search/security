---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usesuperflow-ai-openapi-generated.yml
  format: yaml
  label: Superflow API
  slug: usesuperflow-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usesuperflow-ai/openapi/_ae-authored/usesuperflow-ai-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Superflow
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Superflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Superflow declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Superflow
provider_slug: usesuperflow-ai
scheme_count: 3
schemes:
- evidence: The same key also works as a bearer token on the hosted server.
  name: API key
  type: http-bearer
- evidence: Superflow sends it with each request, and the platform lets it through.
  location: header
  name: Bypass token
  type: other
- evidence: Copy the generated token.
  name: Auth token
  type: http-bearer
slug: usesuperflow-ai-authentication
source_filename: usesuperflow-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://usesuperflow.ai/bug-book/api-key-in-the-thread
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://usesuperflow.ai/bug-book/api-key-in-the-thread\nsources:\n- https://usesuperflow.ai/bug-book/api-key-in-the-thread\n- https://usesuperflow.ai/docs/mcp/api-keys-and-permissions\n- https://usesuperflow.ai/docs/site-access/bypass-token\n- https://usesuperflow.ai/docs/security/auth-tokens\ndescription: Authentication methods documented for Superflow\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: The same key also works as a bearer token on the hosted server.\n- type: other\n  name: Bypass token\n  evidence: Superflow sends it with each request, and the platform lets it through.\n  location: header\n- type: http-bearer\n  name: Auth token\n  evidence: Copy the generated token.\ndocs: https://usesuperflow.ai/bug-book/api-key-in-the-thread\n"
source_yaml_url: https://artifacts.apis.io/usesuperflow-ai/authentication/usesuperflow-ai-authentication.yml
summary_line: 3 schemes
tags:
- QA
- Website Review
- AI Review Agents
- Integrations
- White Label
- Workflow
- Monitoring
- Accessibility
---
