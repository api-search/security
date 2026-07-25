---
api_key_in: []
api_specs:
- filename: tufin-compliance-api-openapi.yml
  format: yaml
  label: Tufin Compliance API
  slug: tufin-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-compliance-api-openapi.yml
- filename: tufin-devices-api-openapi.yml
  format: yaml
  label: Tufin Devices API
  slug: tufin-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-devices-api-openapi.yml
- filename: tufin-objects-api-openapi.yml
  format: yaml
  label: Tufin Objects API
  slug: tufin-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-objects-api-openapi.yml
- filename: tufin-revisions-api-openapi.yml
  format: yaml
  label: Tufin Revisions API
  slug: tufin-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-revisions-api-openapi.yml
- filename: tufin-rules-api-openapi.yml
  format: yaml
  label: Tufin Rules API
  slug: tufin-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-rules-api-openapi.yml
- filename: tufin-tasks-api-openapi.yml
  format: yaml
  label: Tufin Tasks API
  slug: tufin-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-tasks-api-openapi.yml
- filename: tufin-tickets-api-openapi.yml
  format: yaml
  label: Tufin Tickets API
  slug: tufin-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-tickets-api-openapi.yml
- filename: tufin-topology-api-openapi.yml
  format: yaml
  label: Tufin Topology API
  slug: tufin-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-topology-api-openapi.yml
- filename: tufin-users-api-openapi.yml
  format: yaml
  label: Tufin Users API
  slug: tufin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-users-api-openapi.yml
- filename: tufin-workflow-definitions-api-openapi.yml
  format: yaml
  label: Tufin Workflow Definitions API
  slug: tufin-workflow-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-workflow-definitions-api-openapi.yml
- filename: tufin-zones-api-openapi.yml
  format: yaml
  label: Tufin Zones API
  slug: tufin-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-zones-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tufin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tufin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tufin
provider_slug: tufin
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Tufin Orchestration Suite credentials. The authenticated user's TOS permissions apply to all API requests.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tufin-securechange-openapi.yml
  - openapi/tufin-securetrack-openapi.yml
  type: http
slug: tufin-authentication
source_filename: tufin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tufin-securechange-openapi.yml, openapi/tufin-securetrack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Tufin Orchestration Suite credentials. The authenticated\n    user's TOS permissions apply to all API requests.\n  sources:\n  - openapi/tufin-securechange-openapi.yml\n  - openapi/tufin-securetrack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/authentication/tufin-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Compliance
- Firewall Management
- Network Security
- Network Topology
- Policy Orchestration
- Risk Management
- Security Policy Management
- Zero Trust
---
