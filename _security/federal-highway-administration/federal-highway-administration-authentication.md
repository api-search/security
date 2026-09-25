---
anonymous_access: false
api_key_in: []
api_specs:
- filename: federal-highway-administration-authentication-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Authentication API
  slug: federal-highway-administration-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-authentication-api-openapi.yml
- filename: federal-highway-administration-configuration-rest-controller-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Configuration Rest Controller API
  slug: federal-highway-administration-configuration-rest-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-configuration-rest-controller-api-openapi.yml
- filename: federal-highway-administration-deposit-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Deposit API
  slug: federal-highway-administration-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-deposit-api-openapi.yml
- filename: federal-highway-administration-geofence-deployments-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Geofence Deployments API
  slug: federal-highway-administration-geofence-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-geofence-deployments-api-openapi.yml
- filename: federal-highway-administration-geofence-expiration-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Geofence Expiration API
  slug: federal-highway-administration-geofence-expiration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-geofence-expiration-api-openapi.yml
- filename: federal-highway-administration-path-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Path Management API
  slug: federal-highway-administration-path-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-path-management-api-openapi.yml
- filename: federal-highway-administration-registration-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Registration API
  slug: federal-highway-administration-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-registration-api-openapi.yml
- filename: federal-highway-administration-secret-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Secret Management API
  slug: federal-highway-administration-secret-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-secret-management-api-openapi.yml
- filename: federal-highway-administration-tim-configuration-api-openapi.yml
  format: yaml
  label: Federal Highway Administration TIM Configuration API
  slug: federal-highway-administration-tim-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-tim-configuration-api-openapi.yml
- filename: federal-highway-administration-user-limits-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration User Limits Management API
  slug: federal-highway-administration-user-limits-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-user-limits-management-api-openapi.yml
- filename: federal-highway-administration-vendor-limits-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Vendor Limits Management API
  slug: federal-highway-administration-vendor-limits-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-vendor-limits-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Federal Highway Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Highway Administration secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Federal Highway Administration
provider_slug: federal-highway-administration
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Keycloak JWT Bearer Token. Required for all endpoints except decode endpoints. Obtain a token from the /auth/token endpoint using your credentials.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/federal-highway-administration-v2x-app-api-openapi.json
  type: http
slug: federal-highway-administration-authentication
source_filename: federal-highway-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: derived\nsource: openapi/federal-highway-administration-v2x-app-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Keycloak JWT Bearer Token. Required for all endpoints except decode endpoints.\n    Obtain a token from the /auth/token endpoint using your credentials.\n  sources:\n  - openapi/federal-highway-administration-v2x-app-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/authentication/federal-highway-administration-authentication.yml
summary_line: http · 1 scheme
tags:
- Federal Government
- Transportation
- Highways
- Bridge
- Connected Vehicles
- V2X
- Open Source
- Open Data
---
