---
api_key_in: []
api_specs:
- filename: agencyzoom-authentication-api-openapi.yml
  format: yaml
  label: AgencyZoom Authentication API
  slug: agencyzoom-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-authentication-api-openapi.yml
- filename: agencyzoom-configuration-api-openapi.yml
  format: yaml
  label: AgencyZoom Configuration API
  slug: agencyzoom-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-configuration-api-openapi.yml
- filename: agencyzoom-customers-api-openapi.yml
  format: yaml
  label: AgencyZoom Customers API
  slug: agencyzoom-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-customers-api-openapi.yml
- filename: agencyzoom-email-api-openapi.yml
  format: yaml
  label: AgencyZoom Email API
  slug: agencyzoom-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-email-api-openapi.yml
- filename: agencyzoom-leads-api-openapi.yml
  format: yaml
  label: AgencyZoom Leads API
  slug: agencyzoom-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-leads-api-openapi.yml
- filename: agencyzoom-opportunities-api-openapi.yml
  format: yaml
  label: AgencyZoom Opportunities API
  slug: agencyzoom-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-opportunities-api-openapi.yml
- filename: agencyzoom-pipelines-api-openapi.yml
  format: yaml
  label: AgencyZoom Pipelines API
  slug: agencyzoom-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-pipelines-api-openapi.yml
- filename: agencyzoom-policies-api-openapi.yml
  format: yaml
  label: AgencyZoom Policies API
  slug: agencyzoom-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-policies-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agencyzoom Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgencyZoom secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgencyZoom
provider_slug: agencyzoom
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Login via /v1/api/auth/login or /v1/api/auth/ssologin to obtain a JWT, then send as Authorization Bearer.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/agencyzoom-openapi.yml
  type: http
slug: agencyzoom-authentication
source_filename: agencyzoom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agencyzoom-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Login via /v1/api/auth/login or /v1/api/auth/ssologin to obtain a JWT, then send\n    as Authorization Bearer.\n  sources:\n  - openapi/agencyzoom-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/authentication/agencyzoom-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurtech
- CRM
- Sales Automation
- Agency Management
- Customer Retention
---
