---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agilehero-io-account-api-openapi.yml
  format: yaml
  label: AgileHero Account API
  slug: agilehero-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-account-api-openapi.yml
- filename: agilehero-io-cards-api-openapi.yml
  format: yaml
  label: AgileHero Cards API
  slug: agilehero-io-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-cards-api-openapi.yml
- filename: agilehero-io-discovery-api-openapi.yml
  format: yaml
  label: AgileHero Discovery API
  slug: agilehero-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-discovery-api-openapi.yml
- filename: agilehero-io-projects-api-openapi.yml
  format: yaml
  label: AgileHero Projects API
  slug: agilehero-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-projects-api-openapi.yml
- filename: agilehero-io-webhooks-api-openapi.yml
  format: yaml
  label: AgileHero Webhooks API
  slug: agilehero-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for AgileHero as published on the provided pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgileHero Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgileHero declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgileHero
provider_slug: agilehero-io
scheme_count: 2
schemes:
- evidence: Scripts and apps sign in to the API with OAuth, so there's never a key to create, paste, or leak.
  name: OAuth
  type: oauth2
- evidence: An AI client now connects to AgileHero through OAuth, by signing in with your AgileHero account.
  name: OAuth
  type: oauth2
slug: agilehero-io-authentication
source_filename: agilehero-io-authentication.yml
source_heading: Authentication Profile
source_url: https://agilehero.io/changelog/public-rest-api-and-signed-outbound-webhooks/
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agilehero.io/changelog/public-rest-api-and-signed-outbound-webhooks/\nsources:\n- https://agilehero.io/changelog/public-rest-api-and-signed-outbound-webhooks/\n- https://agilehero.io/changelog/oauth-authentication-for-ai-clients-on-the-mcp-server/\ndescription: Authentication schemes for AgileHero as published on the provided pages.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Scripts and apps sign in to the API with OAuth, so there's never a key to create, paste, or leak.\n- type: oauth2\n  name: OAuth\n  evidence: An AI client now connects to AgileHero through OAuth, by signing in with your AgileHero account.\ndocs: https://agilehero.io/changelog/public-rest-api-and-signed-outbound-webhooks/\n"
source_yaml_url: https://artifacts.apis.io/agilehero-io/authentication/agilehero-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Project Management
- Agile
- AI Integration
- Collaboration
---
