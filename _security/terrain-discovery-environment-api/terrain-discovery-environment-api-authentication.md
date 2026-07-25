---
api_key_in:
- header
api_specs:
- filename: terrain-discovery-environment-api-analyses-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Analyses API
  slug: terrain-discovery-environment-api-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-analyses-api-openapi.yml
- filename: terrain-discovery-environment-api-apps-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Apps API
  slug: terrain-discovery-environment-api-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-apps-api-openapi.yml
- filename: terrain-discovery-environment-api-authentication-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Authentication API
  slug: terrain-discovery-environment-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-authentication-api-openapi.yml
- filename: terrain-discovery-environment-api-filesystem-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Filesystem API
  slug: terrain-discovery-environment-api-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-filesystem-api-openapi.yml
- filename: terrain-discovery-environment-api-identifiers-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Identifiers API
  slug: terrain-discovery-environment-api-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-identifiers-api-openapi.yml
- filename: terrain-discovery-environment-api-metadata-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Metadata API
  slug: terrain-discovery-environment-api-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-metadata-api-openapi.yml
- filename: terrain-discovery-environment-api-notifications-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Notifications API
  slug: terrain-discovery-environment-api-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-notifications-api-openapi.yml
- filename: terrain-discovery-environment-api-search-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Search API
  slug: terrain-discovery-environment-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-search-api-openapi.yml
- filename: terrain-discovery-environment-api-sharing-api-openapi.yml
  format: yaml
  label: Terrain Discovery Environment API Sharing API
  slug: terrain-discovery-environment-api-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-discovery-environment-api-sharing-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Terrain Discovery Environment Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terrain Discovery Environment API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Terrain Discovery Environment API
provider_slug: terrain-discovery-environment-api
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer JWT token obtained from Keycloak via /terrain/token/keycloak
  name: KeycloakBearer
  scheme: bearer
  sources:
  - openapi/terrain-openapi.yml
  type: http
- description: Signed JWT token passed in the X-Iplant-De-Jwt header
  in: header
  name: JwtHeader
  parameter: X-Iplant-De-Jwt
  sources:
  - openapi/terrain-openapi.yml
  type: apiKey
slug: terrain-discovery-environment-api-authentication
source_filename: terrain-discovery-environment-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/terrain-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: KeycloakBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer JWT token obtained from Keycloak via /terrain/token/keycloak\n  sources:\n  - openapi/terrain-openapi.yml\n- name: JwtHeader\n  type: apiKey\n  in: header\n  parameter: X-Iplant-De-Jwt\n  description: Signed JWT token passed in the X-Iplant-De-Jwt header\n  sources:\n  - openapi/terrain-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/authentication/terrain-discovery-environment-api-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Bioinformatics
- Data Science
- Life Sciences
- Filesystem
- Cloud Computing
- Open Source
---
