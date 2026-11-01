---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is performed by attaching the API key as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Energyaisolution Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: energyaisolution-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: energyaisolution-com
provider_slug: energyaisolution-com
scheme_count: 1
schemes:
- evidence: Attach your key as a Bearer header.
  header: Authorization
  how_to_obtain: Create an EnergyAI production API key via the create_builder_key endpoint, which returns a live key.
  location: header
  name: Bearer
  type: http-bearer
slug: energyaisolution-com-authentication
source_filename: energyaisolution-com-authentication.yml
source_heading: Authentication Profile
source_url: https://energyaisolution.com/agents
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://energyaisolution.com/agents\nsources:\n- https://energyaisolution.com/agents\ndescription: Authentication is performed by attaching the API key as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Attach your key as a Bearer header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an EnergyAI production API key via the create_builder_key endpoint, which returns a live key.\ndocs: https://energyaisolution.com/agents\n"
source_yaml_url: https://artifacts.apis.io/energyaisolution-com/authentication/energyaisolution-com-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- AI
- DecisionSupport
- RenewableEnergy
- HomeImprovement
---
