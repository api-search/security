---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Agentsync Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Agentsync secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Agentsync
provider_slug: agentsync
scheme_count: 1
schemes:
- description: The ProducerSync REST API authenticates with OAuth 2.0. AgentSync describes the API as using an OAuth 2.0 architecture with encrypted PII, cloud-native (AWS) hosting, and SOC 2 compliance.
  name: OAuth2
  sources:
  - https://agentsync.io/producersync-api
  - https://developer.agentsync.io/api-environments
  type: oauth2
slug: agentsync-authentication
source_filename: agentsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://agentsync.io/producersync-api\ndocs: https://developer.agentsync.io/\nnote: >-\n  No public OpenAPI is available for the ProducerSync API (the developer portal\n  requires registration), so this profile is captured from the provider's public\n  documentation rather than derived from a spec.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials   # machine-to-machine API access; documented as \"OAuth 2.0\" for the ProducerSync REST API\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The ProducerSync REST API authenticates with OAuth 2.0. AgentSync describes\n    the API as using an OAuth 2.0 architecture with encrypted PII, cloud-native\n    (AWS) hosting, and SOC 2 compliance.\n  sources:\n  - https://agentsync.io/producersync-api\n  - https://developer.agentsync.io/api-environments\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentsync/refs/heads/main/authentication/agentsync-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Insurance
- InsurTech
- Compliance
- Producer Management
- Licensing
- NIPR
- REST
- OAuth2
---
