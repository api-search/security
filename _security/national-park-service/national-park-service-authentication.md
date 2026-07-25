---
api_key_in:
- header
api_specs:
- filename: national-park-service-activities-api-openapi.yml
  format: yaml
  label: National Park Service Activities API
  slug: national-park-service-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-activities-api-openapi.yml
- filename: national-park-service-alerts-api-openapi.yml
  format: yaml
  label: National Park Service Alerts API
  slug: national-park-service-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-alerts-api-openapi.yml
- filename: national-park-service-articles-api-openapi.yml
  format: yaml
  label: National Park Service Articles API
  slug: national-park-service-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-articles-api-openapi.yml
- filename: national-park-service-campgrounds-api-openapi.yml
  format: yaml
  label: National Park Service Campgrounds API
  slug: national-park-service-campgrounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-campgrounds-api-openapi.yml
- filename: national-park-service-events-api-openapi.yml
  format: yaml
  label: National Park Service Events API
  slug: national-park-service-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-events-api-openapi.yml
- filename: national-park-service-newsreleases-api-openapi.yml
  format: yaml
  label: National Park Service Newsreleases API
  slug: national-park-service-newsreleases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-newsreleases-api-openapi.yml
- filename: national-park-service-parks-api-openapi.yml
  format: yaml
  label: National Park Service Parks API
  slug: national-park-service-parks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-parks-api-openapi.yml
- filename: national-park-service-people-api-openapi.yml
  format: yaml
  label: National Park Service People API
  slug: national-park-service-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-people-api-openapi.yml
- filename: national-park-service-places-api-openapi.yml
  format: yaml
  label: National Park Service Places API
  slug: national-park-service-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-places-api-openapi.yml
- filename: national-park-service-topics-api-openapi.yml
  format: yaml
  label: National Park Service Topics API
  slug: national-park-service-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-topics-api-openapi.yml
- filename: national-park-service-visitorcenters-api-openapi.yml
  format: yaml
  label: National Park Service Visitorcenters API
  slug: national-park-service-visitorcenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-visitorcenters-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Park Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Park Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Park Service
provider_slug: national-park-service
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/national-park-service-openapi.yml
  type: apiKey
slug: national-park-service-authentication
source_filename: national-park-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-park-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/national-park-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/authentication/national-park-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Conservation
- Federal Government
- Parks
---
