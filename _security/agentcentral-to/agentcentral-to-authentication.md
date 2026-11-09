---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentcentral-to-openapi-generated.yml
  format: yaml
  label: Agent Central API
  slug: agentcentral-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcentral-to/openapi/_ae-authored/agentcentral-to-openapi-generated.yml
auth_types: []
description: Agent Central authenticates API requests using a bearer token API key passed in the Authorization header, and also supports a Connector URL that embeds authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentcentral To Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Central declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Central
provider_slug: agentcentral-to
scheme_count: 1
schemes:
- evidence: Set AGENT_CENTRAL_API_KEY to an ac_live_ key from the dashboard.
  header: Authorization
  how_to_obtain: Create a key in the Agent Central dashboard and copy the ac_live_ key or the Connector URL.
  location: header
  name: API Key
  type: http-bearer
slug: agentcentral-to-authentication
source_filename: agentcentral-to-authentication.yml
source_heading: Authentication Profile
source_url: https://agentcentral.to/docs/best-practices/api-key-scoping
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentcentral.to/docs/best-practices/api-key-scoping\nsources:\n- https://agentcentral.to/docs/best-practices/api-key-scoping\n- https://agentcentral.to/docs/cli/auth\n- https://agentcentral.to/docs/quickstart/claude\n- https://agentcentral.to/docs/quickstart/chatgpt\ndescription: Agent Central authenticates API requests using a bearer token API key passed in the Authorization header, and also supports a Connector\n  URL that embeds authentication.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Set AGENT_CENTRAL_API_KEY to an ac_live_ key from the dashboard.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Agent Central dashboard and copy the ac_live_ key or the Connector URL.\nnote: No OAuth flows, apiKey query/body, or other authentication types are documented on the provided pages.\ndocs: https://agentcentral.to/docs/best-practices/api-key-scoping\n"
source_yaml_url: https://artifacts.apis.io/agentcentral-to/authentication/agentcentral-to-authentication.yml
summary_line: 1 scheme
tags:
- E-Commerce
- Artificial Intelligence
- Automation
- Amazon
- Seller Central
---
