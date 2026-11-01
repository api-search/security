---
anonymous_access: false
api_key_in: []
api_specs:
- filename: immobilienscout24-openapi-generated.yml
  format: yaml
  label: ImmobilienScout24 API
  slug: immobilienscout24-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immobilienscout24/openapi/_ae-authored/immobilienscout24-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Immobilienscout24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: ImmobilienScout24 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ImmobilienScout24
provider_slug: immobilienscout24
scheme_count: 1
schemes:
- description: OAuth 1.0a three-legged flow
  endpoints:
    access_token: /restapi/security/oauth/access_token
    authorize: /restapi/security/oauth/confirm_access
    request_token: /restapi/security/oauth/request_token
  type: oauth1
slug: immobilienscout24-authentication
source_filename: immobilienscout24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://api.immobilienscout24.de/api-docs/authentication/three-legged/\nschemes:\n  - type: oauth1\n    description: OAuth 1.0a three-legged flow\n    endpoints:\n      request_token: /restapi/security/oauth/request_token\n      authorize: /restapi/security/oauth/confirm_access\n      access_token: /restapi/security/oauth/access_token\n"
source_yaml_url: https://artifacts.apis.io/immobilienscout24/authentication/immobilienscout24-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real Estate
- Marketplace
- API
- Germany
- Property Listings
- OAuth
- Search
- Construction Financing
---
