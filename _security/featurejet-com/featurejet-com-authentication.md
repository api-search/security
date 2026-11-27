---
anonymous_access: false
api_key_in: []
api_specs:
- filename: featurejet-com-openapi-generated.yml
  format: yaml
  label: FeatureJet API
  slug: featurejet-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/featurejet-com/openapi/_ae-authored/featurejet-com-openapi-generated.yml
auth_types: []
description: FeatureJet authentication uses an organization‑scoped API key sent as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FeatureJet Authentication
name_suffix: Authentication
oauth_flows: []
overview: FeatureJet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FeatureJet
provider_slug: featurejet-com
scheme_count: 1
schemes:
- evidence: The client sends your key as an Authorization bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the dashboard (API keys page); the raw key is shown once and must be copied.
  location: header
  name: Bearer
  type: http-bearer
slug: featurejet-com-authentication
source_filename: featurejet-com-authentication.yml
source_heading: Authentication Profile
source_url: https://featurejet.com/docs
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://featurejet.com/docs\nsources:\n- https://featurejet.com/docs\n- https://featurejet.com/docs/sdks\n- https://featurejet.com/docs/mcp\ndescription: FeatureJet authentication uses an organization‑scoped API key sent as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The client sends your key as an Authorization bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard (API keys page); the raw key is shown once and must be copied.\ndocs: https://featurejet.com/docs\n"
source_yaml_url: https://artifacts.apis.io/featurejet-com/authentication/featurejet-com-authentication.yml
summary_line: 1 scheme
tags:
- Feedback board
- AI Agents
- Roadmaps
- Software-as-a-Service
---
