---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-location-service-maps-api-openapi.yml
  format: yaml
  label: Amazon Location Service Maps API
  slug: amazon-location-service-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-maps-api-openapi.yml
- filename: amazon-location-service-geofencing-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Geofencing API
  slug: amazon-location-service-geofencing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-geofencing-api-openapi.yml
- filename: amazon-location-service-metadata-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Metadata API
  slug: amazon-location-service-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-metadata-api-openapi.yml
- filename: amazon-location-service-operations-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Operations API
  slug: amazon-location-service-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-operations-api-openapi.yml
- filename: amazon-location-service-places-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Places API
  slug: amazon-location-service-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-places-api-openapi.yml
- filename: amazon-location-service-positions-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Positions API
  slug: amazon-location-service-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-positions-api-openapi.yml
- filename: amazon-location-service-routes-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Routes API
  slug: amazon-location-service-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-routes-api-openapi.yml
- filename: amazon-location-service-tags-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Tags API
  slug: amazon-location-service-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-tags-api-openapi.yml
- filename: amazon-location-service-tracking-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Tracking API
  slug: amazon-location-service-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-tracking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Location Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Location Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Location Service
provider_slug: amazon-location-service
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-location-service-openapi.yml
  type: apiKey
slug: amazon-location-service-authentication
source_filename: amazon-location-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-location-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-location-service-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-location-service/authentication/amazon-location-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- Geofencing
- Location
- Maps
- Routing
---
