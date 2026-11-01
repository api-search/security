---
anonymous_access: false
api_key_in: []
api_specs:
- filename: milestone-openapi-generated.yml
  format: yaml
  label: Milestone API
  slug: milestone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milestone/openapi/_ae-authored/milestone-openapi-generated.yml
auth_types: []
description: Authentication uses a shared secret passed in the request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Milestone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Milestone declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Milestone
provider_slug: milestone
scheme_count: 1
schemes:
- evidence: 'OTEL_HEADERS : "x-shared-secret=<your-shared-secret>"'
  header: x-shared-secret
  location: header
  name: shared secret
  type: apiKey
slug: milestone-authentication
source_filename: milestone-authentication.yml
source_heading: Authentication Profile
source_url: https://mstone.ai/docs/integration-instructions/gen-ai-coding-tools/Lite-LLM/litellm-direct-setup/
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mstone.ai/docs/integration-instructions/gen-ai-coding-tools/Lite-LLM/litellm-direct-setup/\nsources:\n- https://mstone.ai/docs/integration-instructions/gen-ai-coding-tools/Lite-LLM/litellm-direct-setup/\ndescription: Authentication uses a shared secret passed in the request header.\nschemes:\n- type: apiKey\n  name: shared secret\n  evidence: 'OTEL_HEADERS : \"x-shared-secret=<your-shared-secret>\"'\n  location: header\n  header: x-shared-secret\ndocs: https://mstone.ai/docs/integration-instructions/gen-ai-coding-tools/Lite-LLM/litellm-direct-setup/\n"
source_yaml_url: https://artifacts.apis.io/milestone/authentication/milestone-authentication.yml
summary_line: 1 scheme
tags:
- AI Spend
- Agent Governance
- AI Productivity
- AI Governance
- KPI Dashboards
---
