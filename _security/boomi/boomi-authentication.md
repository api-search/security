---
api_key_in: []
api_specs:
- filename: boomi-atoms-api-openapi.yml
  format: yaml
  label: Boomi Atoms API
  slug: boomi-atoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-atoms-api-openapi.yml
- filename: boomi-components-api-openapi.yml
  format: yaml
  label: Boomi Components API
  slug: boomi-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-components-api-openapi.yml
- filename: boomi-deployments-api-openapi.yml
  format: yaml
  label: Boomi Deployments API
  slug: boomi-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-deployments-api-openapi.yml
- filename: boomi-environments-api-openapi.yml
  format: yaml
  label: Boomi Environments API
  slug: boomi-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-environments-api-openapi.yml
- filename: boomi-execution-api-openapi.yml
  format: yaml
  label: Boomi Execution API
  slug: boomi-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-execution-api-openapi.yml
- filename: boomi-golden-records-api-openapi.yml
  format: yaml
  label: Boomi Golden Records API
  slug: boomi-golden-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-golden-records-api-openapi.yml
- filename: boomi-messages-api-openapi.yml
  format: yaml
  label: Boomi Messages API
  slug: boomi-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-messages-api-openapi.yml
- filename: boomi-models-api-openapi.yml
  format: yaml
  label: Boomi Models API
  slug: boomi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-models-api-openapi.yml
- filename: boomi-processes-api-openapi.yml
  format: yaml
  label: Boomi Processes API
  slug: boomi-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-processes-api-openapi.yml
- filename: boomi-quarantine-api-openapi.yml
  format: yaml
  label: Boomi Quarantine API
  slug: boomi-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-quarantine-api-openapi.yml
- filename: boomi-repositories-api-openapi.yml
  format: yaml
  label: Boomi Repositories API
  slug: boomi-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-repositories-api-openapi.yml
- filename: boomi-sources-api-openapi.yml
  format: yaml
  label: Boomi Sources API
  slug: boomi-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-sources-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Boomi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boomi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Boomi
provider_slug: boomi
scheme_count: 2
schemes:
- description: Basic Authentication for the DataHub Platform API. Users with two-factor authentication must include an X-Boomi-OTP header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/boomi-datahub-api-openapi.yml
  - openapi/boomi-platform-rest-api-openapi.yml
  type: http
- description: JWT Bearer token for the Repository API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/boomi-datahub-api-openapi.yml
  - openapi/boomi-event-streams-openapi.yml
  type: http
slug: boomi-authentication
source_filename: boomi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boomi-datahub-api-openapi.yml, openapi/boomi-event-streams-openapi.yml, openapi/boomi-platform-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic Authentication for the DataHub Platform API. Users with two-factor authentication\n    must include an X-Boomi-OTP header.\n  sources:\n  - openapi/boomi-datahub-api-openapi.yml\n  - openapi/boomi-platform-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT Bearer token for the Repository API.\n  sources:\n  - openapi/boomi-datahub-api-openapi.yml\n  - openapi/boomi-event-streams-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/authentication/boomi-authentication.yml
summary_line: http · 2 schemes
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integrations
- Management
- MFT
- Platform
- Workflows
---
