---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: basile-cc-enrichissement-api-openapi.yml
  format: yaml
  label: Basile Enrichissement API
  slug: basile-cc-enrichissement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-enrichissement-api-openapi.yml
- filename: basile-cc-entreprises-api-openapi.yml
  format: yaml
  label: Basile Entreprises API
  slug: basile-cc-entreprises-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-entreprises-api-openapi.yml
- filename: basile-cc-personnes-api-openapi.yml
  format: yaml
  label: Basile Personnes API
  slug: basile-cc-personnes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-personnes-api-openapi.yml
- filename: basile-cc-suggestions-api-openapi.yml
  format: yaml
  label: Basile Suggestions API
  slug: basile-cc-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-suggestions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Basile Cc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basile secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basile
provider_slug: basile-cc
scheme_count: 1
schemes:
- description: 'Clé API en clair (sans `Bearer`). Ex : `Authorization: sk_live_xxxx`.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/original.yaml
  type: apiKey
slug: basile-cc-authentication
source_filename: basile-cc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Clé API en clair (sans `Bearer`). Ex : `Authorization: sk_live_xxxx`.'\n  sources:\n  - openapi/original.yaml\n"
source_yaml_url: https://artifacts.apis.io/basile-cc/authentication/basile-cc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B
- Data
- Leads
- French
- Software-as-a-Service
---
