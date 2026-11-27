---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fluxapay-xyz-openapi-generated.yml
  format: yaml
  label: FluxA API
  slug: fluxapay-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxapay-xyz/openapi/_ae-authored/fluxapay-xyz-openapi-generated.yml
auth_types: []
description: Authentication schemes for FluxA services
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FluxA Authentication
name_suffix: Authentication
oauth_flows: []
overview: FluxA declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FluxA
provider_slug: fluxapay-xyz
scheme_count: 2
schemes:
- evidence: Send the VC as a Bearer token on every AgentCard request.
  header: Authorization
  how_to_obtain: Mint a VC from the Agent ID VC issue endpoint using a login JWT, challenge and audience.
  location: header
  name: Agent VC
  type: http-bearer
- evidence: Model calls, Units, Token Plans and programmatic API publishing on FluxA AgentMarket authenticate with a bearer credential.
  header: Authorization
  how_to_obtain: Create a key in the AgentMarket console (Console > API Keys) or via the API; the raw key is shown once.
  location: header
  name: API Key
  type: http-bearer
slug: fluxapay-xyz-authentication
source_filename: fluxapay-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fluxapay.xyz/agentcard/authentication.html
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fluxapay.xyz/agentcard/authentication.html\nsources:\n- https://docs.fluxapay.xyz/agentcard/authentication.html\n- https://docs.fluxapay.xyz/monetize/api-keys.html\n- https://docs.fluxapay.xyz/monetize/token-plans.html\n- https://docs.fluxapay.xyz/cli/setup.html\ndescription: Authentication schemes for FluxA services\nschemes:\n- type: http-bearer\n  name: Agent VC\n  evidence: Send the VC as a Bearer token on every AgentCard request.\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a VC from the Agent ID VC issue endpoint using a login JWT, challenge and audience.\n- type: http-bearer\n  name: API Key\n  evidence: Model calls, Units, Token Plans and programmatic API publishing on FluxA AgentMarket authenticate with a bearer credential.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the AgentMarket console (Console\
  \ > API Keys) or via the API; the raw key is shown once.\ndocs: https://docs.fluxapay.xyz/agentcard/authentication.html\n"
source_yaml_url: https://artifacts.apis.io/fluxapay-xyz/authentication/fluxapay-xyz-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Artificial Intelligence
- Agents
- Infrastructure
---
