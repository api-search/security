---
anonymous_access: false
api_key_in: []
api_specs:
- filename: m2ml-ai-openapi-generated.yml
  format: yaml
  label: m2ml API
  slug: m2ml-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2ml-ai/openapi/_ae-authored/m2ml-ai-openapi-generated.yml
auth_types: []
description: Authentication methods published on the m2ml documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: m2ml Authentication
name_suffix: Authentication
oauth_flows: []
overview: m2ml declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: m2ml
provider_slug: m2ml-ai
scheme_count: 1
schemes:
- authorize_url: https://api.m2ml.ai/oauth/authorize
  evidence: How to connect to m2ml using OAuth 2.1 instead of a bare API key.
  flows:
  - authorization_code
  how_to_obtain: Dynamic Client Registration via POST https://api.m2ml.ai/oauth/register
  name: OAuth 2.1
  scopes:
  - m2ml:read
  - m2ml:agent
  type: oauth2
slug: m2ml-ai-authentication
source_filename: m2ml-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://m2ml.ai/docs/oauth
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://m2ml.ai/docs/oauth\nsources:\n- https://m2ml.ai/docs/oauth\n- https://m2ml.ai/post/agentic-commerce-readiness-skillmd-web-bot-auth-acp-x402-ap2-cmwhznhbd1e1g11mpnbwnfa3w\n- https://m2ml.ai/post/muse-ember-vs-claude-haiku-55-cost-per-task-beats-price-per-token-cmwhzl8441e0711mph6vqs0sx\ndescription: Authentication methods published on the m2ml documentation.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: How to connect to m2ml using OAuth 2.1 instead of a bare API key.\n  flows:\n  - authorization_code\n  authorize_url: https://api.m2ml.ai/oauth/authorize\n  scopes:\n  - m2ml:read\n  - m2ml:agent\n  how_to_obtain: Dynamic Client Registration via POST https://api.m2ml.ai/oauth/register\ndocs: https://m2ml.ai/docs/oauth\n"
source_yaml_url: https://artifacts.apis.io/m2ml-ai/authentication/m2ml-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Knowledge
- Platform
- Networks
- Open Source
---
