---
anonymous_access: false
api_key_in: []
api_specs:
- filename: distribution-tech-audience-api-openapi.yml
  format: yaml
  label: distribution-tech Audience API
  slug: distribution-tech-audience-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-audience-api-openapi.yml
- filename: distribution-tech-brain-api-openapi.yml
  format: yaml
  label: distribution-tech Brain API
  slug: distribution-tech-brain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-brain-api-openapi.yml
- filename: distribution-tech-campaigns-api-openapi.yml
  format: yaml
  label: distribution-tech Campaigns API
  slug: distribution-tech-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-campaigns-api-openapi.yml
- filename: distribution-tech-creators-api-openapi.yml
  format: yaml
  label: distribution-tech Creators API
  slug: distribution-tech-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-creators-api-openapi.yml
- filename: distribution-tech-evidence-api-openapi.yml
  format: yaml
  label: distribution-tech Evidence API
  slug: distribution-tech-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-evidence-api-openapi.yml
- filename: distribution-tech-feedback-api-openapi.yml
  format: yaml
  label: distribution-tech Feedback API
  slug: distribution-tech-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-feedback-api-openapi.yml
- filename: distribution-tech-inventory-api-openapi.yml
  format: yaml
  label: distribution-tech Inventory API
  slug: distribution-tech-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-inventory-api-openapi.yml
- filename: distribution-tech-plans-api-openapi.yml
  format: yaml
  label: distribution-tech Plans API
  slug: distribution-tech-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-plans-api-openapi.yml
- filename: distribution-tech-results-api-openapi.yml
  format: yaml
  label: distribution-tech Results API
  slug: distribution-tech-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribution-tech/openapi/distribution-tech-results-api-openapi.yml
auth_types: []
description: Authentication schemes for distribution-tech API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Distribution Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: distribution-tech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: distribution-tech
provider_slug: distribution-tech
scheme_count: 1
schemes:
- evidence: Every API and MCP call sends an API key from Developers as a Bearer token.
  header: Authorization
  how_to_obtain: Keys are created, rotated and revoked in your workspace under Developers. A key is shown once when it is created; the workspace keeps only its prefix.
  location: header
  name: Bearer
  type: http-bearer
slug: distribution-tech-authentication
source_filename: distribution-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://distribution.tech/docs/api/authentication
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://distribution.tech/docs/api/authentication\nsources:\n- https://distribution.tech/docs/api/authentication\n- https://distribution.tech/docs/api/authentication.md\n- https://distribution.tech/docs/quickstart\n- https://distribution.tech/docs\ndescription: Authentication schemes for distribution-tech API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every API and MCP call sends an API key from Developers as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are created, rotated and revoked in your workspace under Developers. A key is shown once when it is created; the workspace\n    keeps only its prefix.\ndocs: https://distribution.tech/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/distribution-tech/authentication/distribution-tech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Distribution
- Marketing
- SaaS
- CreatorEconomy
---
