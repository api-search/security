---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: agentsindex-ai-agent-api-openapi.yml
  format: yaml
  label: AgentsIndex Agent API
  slug: agentsindex-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-agent-api-openapi.yml
- filename: agentsindex-ai-agentsindex-machine-api-api-openapi.yml
  format: yaml
  label: AgentsIndex AgentsIndex — Machine API
  slug: agentsindex-ai-agentsindex-machine-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-agentsindex-machine-api-api-openapi.yml
- filename: agentsindex-ai-blog-api-openapi.yml
  format: yaml
  label: AgentsIndex Blog API
  slug: agentsindex-ai-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-blog-api-openapi.yml
- filename: agentsindex-ai-blog-md-api-openapi.yml
  format: yaml
  label: AgentsIndex Blog.md API
  slug: agentsindex-ai-blog-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-blog-md-api-openapi.yml
- filename: agentsindex-ai-categories-api-openapi.yml
  format: yaml
  label: AgentsIndex Categories API
  slug: agentsindex-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-categories-api-openapi.yml
- filename: agentsindex-ai-domain-proof-api-openapi.yml
  format: yaml
  label: AgentsIndex Domain Proof API
  slug: agentsindex-ai-domain-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-domain-proof-api-openapi.yml
- filename: agentsindex-ai-guides-api-openapi.yml
  format: yaml
  label: AgentsIndex Guides API
  slug: agentsindex-ai-guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-guides-api-openapi.yml
- filename: agentsindex-ai-index-json-api-openapi.yml
  format: yaml
  label: AgentsIndex Index.json API
  slug: agentsindex-ai-index-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-index-json-api-openapi.yml
- filename: agentsindex-ai-lead-api-openapi.yml
  format: yaml
  label: AgentsIndex Lead API
  slug: agentsindex-ai-lead-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-lead-api-openapi.yml
- filename: agentsindex-ai-listings-json-api-openapi.yml
  format: yaml
  label: AgentsIndex Listings.json API
  slug: agentsindex-ai-listings-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-listings-json-api-openapi.yml
- filename: agentsindex-ai-llms-full-txt-api-openapi.yml
  format: yaml
  label: AgentsIndex Llms Full.txt API
  slug: agentsindex-ai-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-llms-full-txt-api-openapi.yml
- filename: agentsindex-ai-llms-txt-api-openapi.yml
  format: yaml
  label: AgentsIndex Llms.txt API
  slug: agentsindex-ai-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-llms-txt-api-openapi.yml
- filename: agentsindex-ai-mcp-api-openapi.yml
  format: yaml
  label: AgentsIndex MCP API
  slug: agentsindex-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-mcp-api-openapi.yml
- filename: agentsindex-ai-methodology-md-api-openapi.yml
  format: yaml
  label: AgentsIndex Methodology.md API
  slug: agentsindex-ai-methodology-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-methodology-md-api-openapi.yml
- filename: agentsindex-ai-newsletter-api-openapi.yml
  format: yaml
  label: AgentsIndex Newsletter API
  slug: agentsindex-ai-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-newsletter-api-openapi.yml
- filename: agentsindex-ai-owner-api-openapi.yml
  format: yaml
  label: AgentsIndex Owner API
  slug: agentsindex-ai-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-owner-api-openapi.yml
- filename: agentsindex-ai-search-api-openapi.yml
  format: yaml
  label: AgentsIndex Search API
  slug: agentsindex-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-search-api-openapi.yml
- filename: agentsindex-ai-submissions-api-openapi.yml
  format: yaml
  label: AgentsIndex Submissions API
  slug: agentsindex-ai-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-submissions-api-openapi.yml
- filename: agentsindex-ai-submit-api-openapi.yml
  format: yaml
  label: AgentsIndex Submit API
  slug: agentsindex-ai-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsindex-ai/openapi/agentsindex-ai-submit-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Agentsindex Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentsIndex secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AgentsIndex
provider_slug: agentsindex-ai
scheme_count: 2
schemes:
- description: An agent key the account made at https://agentsindex.ai/dashboard/agents (it starts with mak_). It acts as that account on submit, the claim and domain-proof steps, quotes, orders and reading its own listings, each by the scope the key was given, with the same refusals as its session; it cannot sign in, change the account or pay.
  name: agentKey
  scheme: bearer
  sources:
  - openapi/agentsindex-ai-openapi.json
  type: http
- description: Existing Better Auth session cookie issued through https://agentsindex.ai/login?next=%2Fsubmit. The account email must be verified for submission. This is a session cookie, not an API key to provision.
  in: cookie
  name: sessionCookie
  parameter: __Secure-better-auth.session_token
  sources:
  - openapi/agentsindex-ai-openapi.json
  type: apiKey
slug: agentsindex-ai-authentication
source_filename: agentsindex-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentsindex-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: agentKey\n  type: http\n  scheme: bearer\n  description: An agent key the account made at https://agentsindex.ai/dashboard/agents (it\n    starts with mak_). It acts as that account on submit, the claim and domain-proof steps,\n    quotes, orders and reading its own listings, each by the scope the key was given, with the\n    same refusals as its session; it cannot sign in, change the account or pay.\n  sources:\n  - openapi/agentsindex-ai-openapi.json\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: __Secure-better-auth.session_token\n  description: Existing Better Auth session cookie issued through https://agentsindex.ai/login?next=%2Fsubmit.\n    The account email must be verified for submission. This is a session cookie, not an API\n    key to provision.\n  sources:\n  - openapi/agentsindex-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentsindex-ai/authentication/agentsindex-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Index
- Tools
- Catalog
- Agents
- Marketplace
---
