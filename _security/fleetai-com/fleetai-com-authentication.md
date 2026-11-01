---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fleetai-com-account-api-openapi.yml
  format: yaml
  label: Fleet Account API
  slug: fleetai-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-account-api-openapi.yml
- filename: fleetai-com-browsers-api-openapi.yml
  format: yaml
  label: Fleet Browsers API
  slug: fleetai-com-browsers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-browsers-api-openapi.yml
- filename: fleetai-com-cost-attribution-api-openapi.yml
  format: yaml
  label: Fleet Cost Attribution API
  slug: fleetai-com-cost-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-cost-attribution-api-openapi.yml
- filename: fleetai-com-instances-api-openapi.yml
  format: yaml
  label: Fleet Instances API
  slug: fleetai-com-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-instances-api-openapi.yml
- filename: fleetai-com-jobs-api-openapi.yml
  format: yaml
  label: Fleet Jobs API
  slug: fleetai-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-jobs-api-openapi.yml
- filename: fleetai-com-matg-api-openapi.yml
  format: yaml
  label: Fleet Matg API
  slug: fleetai-com-matg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-matg-api-openapi.yml
- filename: fleetai-com-provenance-audits-api-openapi.yml
  format: yaml
  label: Fleet Provenance Audits API
  slug: fleetai-com-provenance-audits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-provenance-audits-api-openapi.yml
- filename: fleetai-com-seed-gen-api-openapi.yml
  format: yaml
  label: Fleet Seed Gen API
  slug: fleetai-com-seed-gen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-seed-gen-api-openapi.yml
- filename: fleetai-com-seeds-api-openapi.yml
  format: yaml
  label: Fleet Seeds API
  slug: fleetai-com-seeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-seeds-api-openapi.yml
- filename: fleetai-com-sessions-api-openapi.yml
  format: yaml
  label: Fleet Sessions API
  slug: fleetai-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-sessions-api-openapi.yml
- filename: fleetai-com-task-groups-api-openapi.yml
  format: yaml
  label: Fleet Task Groups API
  slug: fleetai-com-task-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-task-groups-api-openapi.yml
- filename: fleetai-com-tasks-api-openapi.yml
  format: yaml
  label: Fleet Tasks API
  slug: fleetai-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-tasks-api-openapi.yml
- filename: fleetai-com-verifiers-api-openapi.yml
  format: yaml
  label: Fleet Verifiers API
  slug: fleetai-com-verifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fleetai-com/openapi/fleetai-com-verifiers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fleetai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fleet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fleet
provider_slug: fleetai-com
scheme_count: 1
schemes:
- description: API key sent as HTTP bearer token. Keys are obtained from the Fleet Platform (https://fleetai.com/dashboard/api-keys), use the prefix sk_ and are read by the SDK from FLEET_API_KEY.
  env_var: FLEET_API_KEY
  key_prefix: sk_
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/fleetai-com-openapi.yml
  type: http
slug: fleetai-com-authentication
source_filename: fleetai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://pypi.org/project/fleet-python/\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/fleetai-com-openapi.yml\n  description: API key sent as HTTP bearer token. Keys are obtained from the Fleet\n    Platform (https://fleetai.com/dashboard/api-keys), use the prefix sk_ and are\n    read by the SDK from FLEET_API_KEY.\n  key_prefix: sk_\n  env_var: FLEET_API_KEY\ndocs: https://pypi.org/project/fleet-python/\nderived_from: openapi/fleetai-com-openapi.yml\nother_methods:\n- name: CLI browser login\n  description: '`flt login` authenticates through the Fleet web app, stores credentials\n    in ~/.fleet/credentials.json and sends JWT auth headers scoped to the selected\n    team; FLEET_API_KEY takes precedence when both are present.'\n"
source_yaml_url: https://artifacts.apis.io/fleetai-com/authentication/fleetai-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Reinforcement Learning Environments
- Evaluations
- Simulation
- Training Data
---
