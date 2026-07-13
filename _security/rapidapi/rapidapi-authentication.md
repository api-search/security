---
api_key_in:
- header
api_specs:
- filename: rapidapi-rest-platform-api-openapi.yml
  format: yaml
  label: RapidAPI REST Platform API
  slug: rapidapi-rest-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-rest-platform-api-openapi.yml
- filename: rapidapi-graphql-platform-api-openapi.yml
  format: yaml
  label: RapidAPI GraphQL Platform API
  slug: rapidapi-graphql-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-graphql-platform-api-openapi.yml
- filename: rapidapi-hub-api-openapi.yml
  format: yaml
  label: RapidAPI Hub API
  slug: rapidapi-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-hub-api-openapi.yml
- filename: rapidapi-testing-api-openapi.yml
  format: yaml
  label: RapidAPI Testing API
  slug: rapidapi-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-testing-api-openapi.yml
- filename: rapidapi-studio-api-openapi.yml
  format: yaml
  label: RapidAPI Studio API
  slug: rapidapi-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-studio-api-openapi.yml
- filename: rapidapi-gateway-api-openapi.yml
  format: yaml
  label: RapidAPI Gateway API
  slug: rapidapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/openapi/rapidapi-gateway-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rapidapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RapidAPI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RapidAPI
provider_slug: rapidapi
scheme_count: 2
schemes:
- description: RapidAPI key used for authenticating requests to the Gateway API.
  in: header
  name: rapidApiKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/rapidapi-gateway-api-openapi.yml
  - openapi/rapidapi-graphql-platform-api-openapi.yml
  - openapi/rapidapi-hub-api-openapi.yml
  - openapi/rapidapi-rest-platform-api-openapi.yml
  - openapi/rapidapi-studio-api-openapi.yml
  - openapi/rapidapi-testing-api-openapi.yml
  type: apiKey
- description: Identity key header required alongside the API key for authorization of GraphQL Platform API requests.
  in: header
  name: rapidApiIdentityKey
  parameter: X-RapidAPI-Identity-Key
  sources:
  - openapi/rapidapi-graphql-platform-api-openapi.yml
  type: apiKey
slug: rapidapi-authentication
source_filename: rapidapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rapidapi-gateway-api-openapi.yml, openapi/rapidapi-graphql-platform-api-openapi.yml,\n  openapi/rapidapi-hub-api-openapi.yml, openapi/rapidapi-rest-platform-api-openapi.yml, openapi/rapidapi-studio-api-openapi.yml,\n  openapi/rapidapi-testing-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rapidApiKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: RapidAPI key used for authenticating requests to the Gateway API.\n  sources:\n  - openapi/rapidapi-gateway-api-openapi.yml\n  - openapi/rapidapi-graphql-platform-api-openapi.yml\n  - openapi/rapidapi-hub-api-openapi.yml\n  - openapi/rapidapi-rest-platform-api-openapi.yml\n  - openapi/rapidapi-studio-api-openapi.yml\n  - openapi/rapidapi-testing-api-openapi.yml\n- name: rapidApiIdentityKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Identity-Key\n  description: Identity key header required\
  \ alongside the API key for authorization of GraphQL\n    Platform API requests.\n  sources:\n  - openapi/rapidapi-graphql-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/authentication/rapidapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Marketplace
- API Management
- API Testing
- API Gateway
- API Design
- Enterprise
---
