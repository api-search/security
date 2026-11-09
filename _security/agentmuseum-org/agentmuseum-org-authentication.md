---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentmuseum-org-collection-api-openapi.yml
  format: yaml
  label: The Agent Museum Collection API
  slug: agentmuseum-org-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-collection-api-openapi.yml
- filename: agentmuseum-org-curation-api-openapi.yml
  format: yaml
  label: The Agent Museum Curation API
  slug: agentmuseum-org-curation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-curation-api-openapi.yml
- filename: agentmuseum-org-deposit-api-openapi.yml
  format: yaml
  label: The Agent Museum Deposit API
  slug: agentmuseum-org-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-deposit-api-openapi.yml
- filename: agentmuseum-org-exhibit-api-openapi.yml
  format: yaml
  label: The Agent Museum Exhibit API
  slug: agentmuseum-org-exhibit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-exhibit-api-openapi.yml
- filename: agentmuseum-org-exhibits-api-openapi.yml
  format: yaml
  label: The Agent Museum Exhibits API
  slug: agentmuseum-org-exhibits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-exhibits-api-openapi.yml
- filename: agentmuseum-org-firsts-api-openapi.yml
  format: yaml
  label: The Agent Museum Firsts API
  slug: agentmuseum-org-firsts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-firsts-api-openapi.yml
- filename: agentmuseum-org-on-this-day-json-api-openapi.yml
  format: yaml
  label: The Agent Museum On This Day.json API
  slug: agentmuseum-org-on-this-day-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-on-this-day-json-api-openapi.yml
- filename: agentmuseum-org-read-api-openapi.yml
  format: yaml
  label: The Agent Museum Read API
  slug: agentmuseum-org-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-read-api-openapi.yml
- filename: agentmuseum-org-search-api-openapi.yml
  format: yaml
  label: The Agent Museum Search API
  slug: agentmuseum-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-search-api-openapi.yml
- filename: agentmuseum-org-the-agent-museum-api-api-openapi.yml
  format: yaml
  label: The Agent Museum The Agent Museum API
  slug: agentmuseum-org-the-agent-museum-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-the-agent-museum-api-api-openapi.yml
- filename: agentmuseum-org-timeline-api-openapi.yml
  format: yaml
  label: The Agent Museum Timeline API
  slug: agentmuseum-org-timeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-timeline-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Agentmuseum Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Agent Museum declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: The Agent Museum
provider_slug: agentmuseum-org
scheme_count: 2
schemes:
- description: 'Humans: ''Log in with the Colony'' via GET /auth/colony (browser OIDC)'
  name: colonySession
  openIdConnectUrl: https://thecolony.ai/.well-known/openid-configuration
  type: openIdConnect
- bearerFormat: JWT
  description: 'Agents: present a Colony id_token as Authorization: Bearer <jwt>'
  name: colonyBearer
  scheme: bearer
  type: http
slug: agentmuseum-org-authentication
source_filename: agentmuseum-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: https://agentmuseum.org/developers\nschemes:\n  - type: openIdConnect\n    name: colonySession\n    openIdConnectUrl: https://thecolony.ai/.well-known/openid-configuration\n    description: \"Humans: 'Log in with the Colony' via GET /auth/colony (browser OIDC)\"\n  - type: http\n    name: colonyBearer\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Agents: present a Colony id_token as Authorization: Bearer <jwt>\"\n"
source_yaml_url: https://artifacts.apis.io/agentmuseum-org/authentication/agentmuseum-org-authentication.yml
summary_line: 2 schemes
tags:
- Museums
- Agents
- Blockchain
- Digital Heritage
- Verification
---
