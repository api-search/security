---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scento-contrast-api-openapi.yml
  format: yaml
  label: Scento Compendium API Contrast API
  slug: scento-contrast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-contrast-api-openapi.yml
- filename: scento-perfume-portrait-api-openapi.yml
  format: yaml
  label: Scento Compendium API Perfume portrait API
  slug: scento-perfume-portrait-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-perfume-portrait-api-openapi.yml
- filename: scento-scent-neighbours-api-openapi.yml
  format: yaml
  label: Scento Compendium API Scent neighbours API
  slug: scento-scent-neighbours-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-scent-neighbours-api-openapi.yml
- filename: scento-search-the-compendium-api-openapi.yml
  format: yaml
  label: Scento Compendium API Search the Compendium API
  slug: scento-search-the-compendium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-search-the-compendium-api-openapi.yml
- filename: scento-get-a-perfume-s-notes-and-profile-api-openapi.yml
  format: yaml
  label: Scento Compendium API Get a perfume's notes and profile API
  slug: scento-get-a-perfume-s-notes-and-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-get-a-perfume-s-notes-and-profile-api-openapi.yml
- filename: scento-search-perfumes-houses-and-notes-api-openapi.yml
  format: yaml
  label: Scento Compendium API Search perfumes, houses and notes API
  slug: scento-search-perfumes-houses-and-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-search-perfumes-houses-and-notes-api-openapi.yml
auth_types: []
description: Scento uses OAuth 2.0 with multiple grant types and client authentication methods.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Scento Compendium API Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scento Compendium API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Scento Compendium API
provider_slug: scento
scheme_count: 1
schemes:
- evidence: '"token_endpoint_auth_methods_supported": [ "none", "client_secret_basic", "client_secret_post" ]'
  header: Authorization
  how_to_obtain: Obtain client_secret during client registration and include it in HTTP Basic auth when calling the token or revocation endpoints.
  location: header
  name: client_secret_basic
  type: http-basic
slug: scento-authentication
source_filename: scento-authentication.yml
source_heading: Authentication Profile
source_url: https://www.scento.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.scento.com/.well-known/oauth-authorization-server\nsources:\n- https://www.scento.com/.well-known/oauth-authorization-server\n- https://www.scento.com/auth.md\ndescription: Scento uses OAuth 2.0 with multiple grant types and client authentication methods.\nschemes:\n- type: http-basic\n  name: client_secret_basic\n  evidence: '\"token_endpoint_auth_methods_supported\": [ \"none\", \"client_secret_basic\", \"client_secret_post\" ]'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain client_secret during client registration and include it in HTTP Basic auth when calling the token or revocation endpoints.\nnote: No other authentication schemes (apiKey, jwt, hmac, mtls, other) are documented. 2 extracted row(s) were dropped because their quote was\n  not on the page.\ndocs: https://www.scento.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/scento/authentication/scento-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-Commerce
- Fragrance
- Decant
---
