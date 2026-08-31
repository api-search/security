---
api_key_in:
- header
api_specs:
- filename: university-of-calgary-auroral-transport-model-atm-api-openapi.yml
  format: yaml
  label: University of Calgary Auroral Transport Model (ATM) API
  slug: university-of-calgary-auroral-transport-model-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-auroral-transport-model-atm-api-openapi.yml
- filename: university-of-calgary-data-distribution-api-openapi.yml
  format: yaml
  label: University of Calgary Data Distribution API
  slug: university-of-calgary-data-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-data-distribution-api-openapi.yml
- filename: university-of-calgary-hapi-api-openapi.yml
  format: yaml
  label: University of Calgary SRS HAPI (Heliophysics API) Server
  slug: university-of-calgary-hapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-hapi-api-openapi.yml
- filename: university-of-calgary-operations-sitl-api-openapi.yml
  format: yaml
  label: University of Calgary Operations - SITL API
  slug: university-of-calgary-operations-sitl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-operations-sitl-api-openapi.yml
- filename: university-of-calgary-real-time-data-api-openapi.yml
  format: yaml
  label: University of Calgary Real-Time Data API
  slug: university-of-calgary-real-time-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-real-time-data-api-openapi.yml
- filename: university-of-calgary-utilities-api-openapi.yml
  format: yaml
  label: University of Calgary Utilities API
  slug: university-of-calgary-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-utilities-api-openapi.yml
- filename: university-of-calgary-application-wadl-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Application.wadl API
  slug: university-of-calgary-application-wadl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-application-wadl-api-openapi.yml
- filename: university-of-calgary-authenticate-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Authenticate API
  slug: university-of-calgary-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-authenticate-api-openapi.yml
- filename: university-of-calgary-availability-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Availability API
  slug: university-of-calgary-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-availability-api-openapi.yml
- filename: university-of-calgary-conjunction-search-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Conjunction Search API
  slug: university-of-calgary-conjunction-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-conjunction-search-api-openapi.yml
- filename: university-of-calgary-data-products-search-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Data Products Search API
  slug: university-of-calgary-data-products-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-data-products-search-api-openapi.yml
- filename: university-of-calgary-data-sources-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Data Sources API
  slug: university-of-calgary-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-data-sources-api-openapi.yml
- filename: university-of-calgary-ephemeris-search-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Ephemeris Search API
  slug: university-of-calgary-ephemeris-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-ephemeris-search-api-openapi.yml
- filename: university-of-calgary-manage-data-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Manage Data API
  slug: university-of-calgary-manage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-manage-data-api-openapi.yml
- filename: university-of-calgary-utils-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Utils API
  slug: university-of-calgary-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-utils-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Calgary Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Calgary secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Calgary
provider_slug: university-of-calgary
scheme_count: 3
schemes:
- bearerFormat: Generated by server
  description: Send the Authorization header found in the response of a successful /authentication request on all  secure endpoints. Copy it verbatim to the request header. It is fine to send this header on all requests  to the API. The value in Swagger UI should only include the access token part (leave out 'Bearer').
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/university-of-calgary-aurorax-api.yaml
  - openapi/university-of-calgary-srs-api.yaml
  type: http
- description: API keys are intended to be used by non-interactive software interfacing with the REST API. These can  be used instead of an Access Token approach.
  in: header
  name: ApiKeyAuth
  parameter: x-aurorax-api-key
  sources:
  - openapi/university-of-calgary-aurorax-api.yaml
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: x-srs-api-key
  sources:
  - openapi/university-of-calgary-srs-api.yaml
  type: apiKey
slug: university-of-calgary-authentication
source_filename: university-of-calgary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-calgary-aurorax-api.yaml, openapi/university-of-calgary-srs-api.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: Generated by server\n  description: Send the Authorization header found in the response of a successful /authentication\n    request on all  secure endpoints. Copy it verbatim to the request header. It is fine to\n    send this header on all requests  to the API. The value in Swagger UI should only include\n    the access token part (leave out 'Bearer').\n  sources:\n  - openapi/university-of-calgary-aurorax-api.yaml\n  - openapi/university-of-calgary-srs-api.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-aurorax-api-key\n  description: API keys are intended to be used by non-interactive software interfacing with\n    the REST API. These can  be used instead of an Access\
  \ Token approach.\n  sources:\n  - openapi/university-of-calgary-aurorax-api.yaml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-srs-api-key\n  sources:\n  - openapi/university-of-calgary-srs-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/authentication/university-of-calgary-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Education
- Higher Education
- University
- Public Research University
- Canada
- Alberta
- U15
- Research
- Research Data
- Open Access
- Repository
- OAI-PMH
- Identity Federation
- Research Computing
- Space Physics
- Heliophysics
- Open Data
---
