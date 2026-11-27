---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tenor-autocomplete-api-openapi.yml
  format: yaml
  label: Tenor Autocomplete API
  slug: tenor-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-autocomplete-api-openapi.yml
- filename: tenor-categories-api-openapi.yml
  format: yaml
  label: Tenor Categories API
  slug: tenor-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-categories-api-openapi.yml
- filename: tenor-featured-api-openapi.yml
  format: yaml
  label: Tenor Featured API
  slug: tenor-featured-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-featured-api-openapi.yml
- filename: tenor-posts-api-openapi.yml
  format: yaml
  label: Tenor Posts API
  slug: tenor-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-posts-api-openapi.yml
- filename: tenor-registershare-api-openapi.yml
  format: yaml
  label: Tenor Registershare API
  slug: tenor-registershare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-registershare-api-openapi.yml
- filename: tenor-search-api-openapi.yml
  format: yaml
  label: Tenor Search API
  slug: tenor-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-search-api-openapi.yml
- filename: tenor-search-suggestions-api-openapi.yml
  format: yaml
  label: Tenor Search Suggestions API
  slug: tenor-search-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-search-suggestions-api-openapi.yml
- filename: tenor-trending-terms-api-openapi.yml
  format: yaml
  label: Tenor Trending Terms API
  slug: tenor-trending-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenor/openapi/tenor-trending-terms-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tenor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tenor declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tenor
provider_slug: tenor
scheme_count: 2
schemes:
- description: Google Cloud API key created in the Google Cloud Console (APIs & Services > Credentials) with the Tenor API enabled; the docs recommend restricting keys to the necessary APIs only.
  in: query
  name: key
  type: apiKey
- description: Optional integration identifier; not a credential.
  in: query
  name: client_key
  type: client-identifier
slug: tenor-authentication
source_filename: tenor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Tenor authentication\ngenerated: '2026-11-11'\nmethod: searched\nsource: https://developers.google.com/tenor/guides/quickstart\ndocs: https://developers.google.com/tenor/guides/quickstart\nschemes:\n- type: apiKey\n  in: query\n  name: key\n  description: Google Cloud API key created in the Google Cloud Console (APIs & Services > Credentials) with the Tenor API enabled; the docs recommend restricting keys to the necessary APIs only.\n- type: client-identifier\n  in: query\n  name: client_key\n  description: Optional integration identifier; not a credential.\nnote: As of Jan 2026 Google no longer accepts new Tenor API clients, so no new key can be obtained.\n"
source_yaml_url: https://artifacts.apis.io/tenor/authentication/tenor-authentication.yml
summary_line: 2 schemes
tags:
- GIFs
- Animated Images
- Search
- Media
- Google
---
