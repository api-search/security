---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flowra-dev-auth-configs-api-openapi.yml
  format: yaml
  label: Flowra Auth Configs API
  slug: flowra-dev-auth-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-auth-configs-api-openapi.yml
- filename: flowra-dev-browser-api-openapi.yml
  format: yaml
  label: Flowra Browser API
  slug: flowra-dev-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-browser-api-openapi.yml
- filename: flowra-dev-chat-api-openapi.yml
  format: yaml
  label: Flowra Chat API
  slug: flowra-dev-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-chat-api-openapi.yml
- filename: flowra-dev-connected-accounts-api-openapi.yml
  format: yaml
  label: Flowra Connected Accounts API
  slug: flowra-dev-connected-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-connected-accounts-api-openapi.yml
- filename: flowra-dev-external-users-api-openapi.yml
  format: yaml
  label: Flowra External Users API
  slug: flowra-dev-external-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-external-users-api-openapi.yml
- filename: flowra-dev-file-api-openapi.yml
  format: yaml
  label: Flowra File API
  slug: flowra-dev-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-file-api-openapi.yml
- filename: flowra-dev-knowledge-api-openapi.yml
  format: yaml
  label: Flowra Knowledge API
  slug: flowra-dev-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-knowledge-api-openapi.yml
- filename: flowra-dev-llm-api-openapi.yml
  format: yaml
  label: Flowra LLM API
  slug: flowra-dev-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-llm-api-openapi.yml
- filename: flowra-dev-mcp-api-openapi.yml
  format: yaml
  label: Flowra MCP API
  slug: flowra-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-mcp-api-openapi.yml
- filename: flowra-dev-sandbox-api-openapi.yml
  format: yaml
  label: Flowra Sandbox API
  slug: flowra-dev-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-sandbox-api-openapi.yml
- filename: flowra-dev-skills-api-openapi.yml
  format: yaml
  label: Flowra Skills API
  slug: flowra-dev-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-skills-api-openapi.yml
- filename: flowra-dev-table-api-openapi.yml
  format: yaml
  label: Flowra Table API
  slug: flowra-dev-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-table-api-openapi.yml
- filename: flowra-dev-toolkits-api-openapi.yml
  format: yaml
  label: Flowra Toolkits API
  slug: flowra-dev-toolkits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-toolkits-api-openapi.yml
- filename: flowra-dev-tools-api-openapi.yml
  format: yaml
  label: Flowra Tools API
  slug: flowra-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-tools-api-openapi.yml
- filename: flowra-dev-triggers-api-openapi.yml
  format: yaml
  label: Flowra Triggers API
  slug: flowra-dev-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-triggers-api-openapi.yml
- filename: flowra-dev-usage-api-openapi.yml
  format: yaml
  label: Flowra Usage API
  slug: flowra-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-usage-api-openapi.yml
- filename: flowra-dev-users-api-openapi.yml
  format: yaml
  label: Flowra Users API
  slug: flowra-dev-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-users-api-openapi.yml
- filename: flowra-dev-workflow-agent-api-openapi.yml
  format: yaml
  label: Flowra Workflow & Agent API
  slug: flowra-dev-workflow-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowra-dev/openapi/flowra-dev-workflow-agent-api-openapi.yml
auth_types: []
description: Authentication for Flowra API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Flowra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flowra declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Flowra
provider_slug: flowra-dev
scheme_count: 1
schemes:
- evidence: 'Optional: x-username header

    For endpoints that support it, send **x-username** to act as an end user (external user) inside your project.'
  header: x-username
  how_to_obtain: Use the external user’s stable username (e.g., customer_alice) when needed.
  location: header
  name: x-username
  type: apiKey
slug: flowra-dev-authentication
source_filename: flowra-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.flowra.dev/product/projects-and-keys.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.flowra.dev/product/projects-and-keys.md\nsources:\n- https://docs.flowra.dev/product/projects-and-keys.md\n- https://docs.flowra.dev/authentication.md\n- https://docs.flowra.dev/api-reference/workflow-&-agent/add-connection-after-oauth-for-a-workflow.md\n- https://docs.flowra.dev/api-reference/usage/credit-usage-ledger-api-key.md\ndescription: Authentication for Flowra API\nschemes:\n- type: apiKey\n  name: x-username\n  evidence: 'Optional: x-username header\n\n    For endpoints that support it, send **x-username** to act as an end user (external user) inside your project.'\n  location: header\n  header: x-username\n  how_to_obtain: Use the external user’s stable username (e.g., customer_alice) when needed.\nnote: No OAuth2 flows are documented for Flowra API. 2 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://docs.flowra.dev/product/projects-and-keys.md\n"
source_yaml_url: https://artifacts.apis.io/flowra-dev/authentication/flowra-dev-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Automation
- Workflows
- Low-Code
- Integration
---
