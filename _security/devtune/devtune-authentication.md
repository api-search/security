---
anonymous_access: false
api_key_in: []
api_specs:
- filename: devtune-accuracy-api-openapi.yml
  format: yaml
  label: DevTune Accuracy API
  slug: devtune-accuracy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-accuracy-api-openapi.yml
- filename: devtune-actions-api-openapi.yml
  format: yaml
  label: DevTune Actions API
  slug: devtune-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-actions-api-openapi.yml
- filename: devtune-adoption-api-openapi.yml
  format: yaml
  label: DevTune Adoption API
  slug: devtune-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-adoption-api-openapi.yml
- filename: devtune-agent-picks-api-openapi.yml
  format: yaml
  label: DevTune Agent Picks API
  slug: devtune-agent-picks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-agent-picks-api-openapi.yml
- filename: devtune-agent-registration-api-openapi.yml
  format: yaml
  label: DevTune Agent registration API
  slug: devtune-agent-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-agent-registration-api-openapi.yml
- filename: devtune-agents-api-openapi.yml
  format: yaml
  label: DevTune Agents API
  slug: devtune-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-agents-api-openapi.yml
- filename: devtune-ai-traffic-api-openapi.yml
  format: yaml
  label: DevTune AI Traffic API
  slug: devtune-ai-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-ai-traffic-api-openapi.yml
- filename: devtune-audit-and-pages-api-openapi.yml
  format: yaml
  label: DevTune Audit and pages API
  slug: devtune-audit-and-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-audit-and-pages-api-openapi.yml
- filename: devtune-citations-api-openapi.yml
  format: yaml
  label: DevTune Citations API
  slug: devtune-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-citations-api-openapi.yml
- filename: devtune-connection-and-usage-api-openapi.yml
  format: yaml
  label: DevTune Connection and usage API
  slug: devtune-connection-and-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-connection-and-usage-api-openapi.yml
- filename: devtune-content-gaps-api-openapi.yml
  format: yaml
  label: DevTune Content gaps API
  slug: devtune-content-gaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-content-gaps-api-openapi.yml
- filename: devtune-dex-api-openapi.yml
  format: yaml
  label: DevTune Dex API
  slug: devtune-dex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-dex-api-openapi.yml
- filename: devtune-library-and-knowledge-api-openapi.yml
  format: yaml
  label: DevTune Library and Knowledge API
  slug: devtune-library-and-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-library-and-knowledge-api-openapi.yml
- filename: devtune-positioning-api-openapi.yml
  format: yaml
  label: DevTune Positioning API
  slug: devtune-positioning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-positioning-api-openapi.yml
- filename: devtune-prompts-and-topics-api-openapi.yml
  format: yaml
  label: DevTune Prompts and topics API
  slug: devtune-prompts-and-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-prompts-and-topics-api-openapi.yml
- filename: devtune-results-api-openapi.yml
  format: yaml
  label: DevTune Results API
  slug: devtune-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-results-api-openapi.yml
- filename: devtune-setup-api-openapi.yml
  format: yaml
  label: DevTune Setup API
  slug: devtune-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-setup-api-openapi.yml
- filename: devtune-visibility-api-openapi.yml
  format: yaml
  label: DevTune Visibility API
  slug: devtune-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-visibility-api-openapi.yml
- filename: devtune-webhooks-api-openapi.yml
  format: yaml
  label: DevTune Webhooks API
  slug: devtune-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for DevTune API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DevTune Authentication
name_suffix: Authentication
oauth_flows: []
overview: DevTune declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DevTune
provider_slug: devtune
scheme_count: 1
schemes:
- evidence: The DevTune API accepts project API keys in the `Authorization` header.
  header: Authorization
  how_to_obtain: Create a project‑scoped API key in the DevTune account UI under API Keys; the full key is shown once after creation.
  location: header
  name: API Key
  scopes:
  - visibility.read
  - citations.read
  - competitive.read
  - positioning.read
  - accuracy.read
  - adoption.read
  - traffic.read
  - referrals.read
  - pages.read
  - audit.read
  - outcomes.read
  - intelligence.read
  - actions.read
  - actions.write
  - prompts.write
  - setup.read
  - setup.write
  - library.read
  - library.write
  - agents.read
  - agents.run
  - agents.review
  - agents.write
  - agent_picks.run
  - webhooks.read
  - webhooks.write
  type: http-bearer
slug: devtune-authentication
source_filename: devtune-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.devtune.ai/account-billing/api-keys.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.devtune.ai/account-billing/api-keys.md\nsources:\n- https://docs.devtune.ai/account-billing/api-keys.md\n- https://docs.devtune.ai/api-reference/authentication.md\n- https://docs.devtune.ai/api-reference/revoke-the-calling-api-key.md\n- https://docs.devtune.ai/api-reference/rotate-the-calling-api-key.md\ndescription: Authentication schemes for DevTune API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: The DevTune API accepts project API keys in the `Authorization` header.\n  location: header\n  header: Authorization\n  scopes:\n  - visibility.read\n  - citations.read\n  - competitive.read\n  - positioning.read\n  - accuracy.read\n  - adoption.read\n  - traffic.read\n  - referrals.read\n  - pages.read\n  - audit.read\n  - outcomes.read\n  - intelligence.read\n  - actions.read\n  - actions.write\n  - prompts.write\n  - setup.read\n  - setup.write\n  - library.read\n\
  \  - library.write\n  - agents.read\n  - agents.run\n  - agents.review\n  - agents.write\n  - agent_picks.run\n  - webhooks.read\n  - webhooks.write\n  how_to_obtain: Create a project‑scoped API key in the DevTune account UI under API Keys; the full key is shown once after creation.\nnote: No OAuth2 flows are documented on the provided pages.\ndocs: https://docs.devtune.ai/account-billing/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/devtune/authentication/devtune-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Search
- Analytics
- Platform
---
