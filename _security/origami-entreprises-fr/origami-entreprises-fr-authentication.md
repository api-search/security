---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: origami-entreprises-fr-alertes-webhooks-api-openapi.yml
  format: yaml
  label: Origami Entreprises Alertes (webhooks) API
  slug: origami-entreprises-fr-alertes-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/origami-entreprises-fr/openapi/origami-entreprises-fr-alertes-webhooks-api-openapi.yml
- filename: origami-entreprises-fr-dirigeant-api-openapi.yml
  format: yaml
  label: Origami Entreprises Dirigeant API
  slug: origami-entreprises-fr-dirigeant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/origami-entreprises-fr/openapi/origami-entreprises-fr-dirigeant-api-openapi.yml
- filename: origami-entreprises-fr-entreprise-api-openapi.yml
  format: yaml
  label: Origami Entreprises Entreprise API
  slug: origami-entreprises-fr-entreprise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/origami-entreprises-fr/openapi/origami-entreprises-fr-entreprise-api-openapi.yml
- filename: origami-entreprises-fr-entreprises-api-openapi.yml
  format: yaml
  label: Origami Entreprises Entreprises API
  slug: origami-entreprises-fr-entreprises-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/origami-entreprises-fr/openapi/origami-entreprises-fr-entreprises-api-openapi.yml
- filename: origami-entreprises-fr-suggestions-api-openapi.yml
  format: yaml
  label: Origami Entreprises Suggestions API
  slug: origami-entreprises-fr-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/origami-entreprises-fr/openapi/origami-entreprises-fr-suggestions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Origami Entreprises Authentication
name_suffix: Authentication
oauth_flows: []
overview: Origami Entreprises secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Origami Entreprises
provider_slug: origami-entreprises-fr
scheme_count: 2
schemes:
- bearerFormat: ori_mcp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  description: Clé API au format `ori_mcp_…`. Obtenue via [/account/api-keys/](/account/api-keys/). Une seule clé donne accès à l'API REST et au serveur MCP.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/origami-entreprises-fr-openapi.yaml
  - openapi/origami-entreprises-fr.yaml
  type: http
- description: 'Alternative à `Authorization: Bearer <key>`.'
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/origami-entreprises-fr-openapi.yaml
  - openapi/origami-entreprises-fr.yaml
  type: apiKey
slug: origami-entreprises-fr-authentication
source_filename: origami-entreprises-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/origami-entreprises-fr-openapi.yaml, openapi/origami-entreprises-fr.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ori_mcp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n  description: Clé API au format `ori_mcp_…`. Obtenue via [/account/api-keys/](/account/api-keys/).\n    Une seule clé donne accès à l'API REST et au serveur MCP.\n  sources:\n  - openapi/origami-entreprises-fr-openapi.yaml\n  - openapi/origami-entreprises-fr.yaml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Alternative à `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/origami-entreprises-fr-openapi.yaml\n  - openapi/origami-entreprises-fr.yaml\n"
source_yaml_url: https://artifacts.apis.io/origami-entreprises-fr/authentication/origami-entreprises-fr-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Data
- French
- Business
---
