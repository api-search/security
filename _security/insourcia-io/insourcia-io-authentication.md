---
anonymous_access: false
api_key_in: []
api_specs:
- filename: insourcia-io-auth-api-openapi.yml
  format: yaml
  label: Insourcia Auth API
  slug: insourcia-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-auth-api-openapi.yml
- filename: insourcia-io-company-api-openapi.yml
  format: yaml
  label: Insourcia Company API
  slug: insourcia-io-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-company-api-openapi.yml
- filename: insourcia-io-directors-api-openapi.yml
  format: yaml
  label: Insourcia Directors API
  slug: insourcia-io-directors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-directors-api-openapi.yml
- filename: insourcia-io-documents-api-openapi.yml
  format: yaml
  label: Insourcia Documents API
  slug: insourcia-io-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-documents-api-openapi.yml
- filename: insourcia-io-events-api-openapi.yml
  format: yaml
  label: Insourcia Events API
  slug: insourcia-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-events-api-openapi.yml
- filename: insourcia-io-financials-api-openapi.yml
  format: yaml
  label: Insourcia Financials API
  slug: insourcia-io-financials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-financials-api-openapi.yml
- filename: insourcia-io-search-api-openapi.yml
  format: yaml
  label: Insourcia Search API
  slug: insourcia-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-search-api-openapi.yml
- filename: insourcia-io-veille-api-openapi.yml
  format: yaml
  label: Insourcia Veille API
  slug: insourcia-io-veille-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-veille-api-openapi.yml
- filename: insourcia-io-webhooks-api-openapi.yml
  format: yaml
  label: Insourcia Webhooks API
  slug: insourcia-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insourcia-io/openapi/insourcia-io-webhooks-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Insourcia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insourcia declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Insourcia
provider_slug: insourcia-io
scheme_count: 1
schemes:
- evidence: 'Chaque requête porte un en-tête Authorization: Bearer <token>. Deux types de jetons sont acceptés : Clé API (format isk_xxx) : à créer dans l''application, rubrique Paramètres > API / MCP (https://app.insourcia.io/settings/api) ; JWT OAuth 2.1 : obtenu par le parcours OAuth du serveur MCP.'
  header: Authorization
  how_to_obtain: Clé API (format isk_xxx) créée dans les paramètres de l'application ou JWT OAuth 2.1 obtenu via le parcours OAuth du serveur MCP.
  location: header
  name: Bearer
  type: http-bearer
slug: insourcia-io-authentication
source_filename: insourcia-io-authentication.yml
source_heading: Authentication Profile
source_url: https://insourcia.io/docs/api-reference/#tag/auth
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://insourcia.io/docs/api-reference/#tag/auth\nsources:\n- https://insourcia.io/docs/api-reference/#tag/auth\n- https://insourcia.io/docs/api-reference/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Chaque requête porte un en-tête Authorization: Bearer <token>. Deux types de jetons sont acceptés : Clé API (format isk_xxx) : à\n    créer dans l''application, rubrique Paramètres > API / MCP (https://app.insourcia.io/settings/api) ; JWT OAuth 2.1 : obtenu par le parcours\n    OAuth du serveur MCP.'\n  location: header\n  header: Authorization\n  how_to_obtain: Clé API (format isk_xxx) créée dans les paramètres de l'application ou JWT OAuth 2.1 obtenu via le parcours OAuth du serveur\n    MCP.\ndocs: https://insourcia.io/docs/api-reference/#tag/auth\n"
source_yaml_url: https://artifacts.apis.io/insourcia-io/authentication/insourcia-io-authentication.yml
summary_line: 1 scheme
tags:
- Private Market Intelligence
- AI Integration
- Financial Data
- Company Search
- Risk Assessment
---
