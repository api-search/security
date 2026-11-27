---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kaneme-com-certificat-api-openapi.yml
  format: yaml
  label: Kaneme Certificat API
  slug: kaneme-com-certificat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-certificat-api-openapi.yml
- filename: kaneme-com-compte-api-openapi.yml
  format: yaml
  label: Kaneme Compte API
  slug: kaneme-com-compte-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-compte-api-openapi.yml
- filename: kaneme-com-criture-api-openapi.yml
  format: yaml
  label: Kaneme Écriture API
  slug: kaneme-com-criture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-criture-api-openapi.yml
- filename: kaneme-com-cycle-de-vie-api-openapi.yml
  format: yaml
  label: Kaneme Cycle de vie API
  slug: kaneme-com-cycle-de-vie-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-cycle-de-vie-api-openapi.yml
- filename: kaneme-com-documents-api-openapi.yml
  format: yaml
  label: Kaneme Documents API
  slug: kaneme-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-documents-api-openapi.yml
- filename: kaneme-com-mesure-api-openapi.yml
  format: yaml
  label: Kaneme Mesure API
  slug: kaneme-com-mesure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-mesure-api-openapi.yml
- filename: kaneme-com-projets-api-openapi.yml
  format: yaml
  label: Kaneme Projets API
  slug: kaneme-com-projets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-projets-api-openapi.yml
- filename: kaneme-com-voix-api-openapi.yml
  format: yaml
  label: Kaneme Voix API
  slug: kaneme-com-voix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaneme-com/openapi/kaneme-com-voix-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kaneme Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaneme declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kaneme
provider_slug: kaneme-com
scheme_count: 2
schemes:
- evidence: 'Credential Authorization: Bearer kaneme_…'
  header: Authorization
  location: header
  name: API key
  type: http-bearer
- evidence: Credential Authorization code followed by a short lived access token.
  name: OAuth
  type: oauth2
slug: kaneme-com-authentication
source_filename: kaneme-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kaneme.com/en/developers/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kaneme.com/en/developers/authentication\nsources:\n- https://kaneme.com/en/developers/authentication\n- https://kaneme.com/en/developers\n- https://kaneme.com/en\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Credential Authorization: Bearer kaneme_…'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth\n  evidence: Credential Authorization code followed by a short lived access token.\ndocs: https://kaneme.com/en/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/kaneme-com/authentication/kaneme-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Voice
- Personalization
---
