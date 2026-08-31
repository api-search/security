---
api_key_in: []
api_specs:
- filename: politecnico-di-torino-announcements-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Announcements API
  slug: politecnico-di-torino-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-announcements-api-openapi.yml
- filename: politecnico-di-torino-auth-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Auth API
  slug: politecnico-di-torino-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-auth-api-openapi.yml
- filename: politecnico-di-torino-bookings-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Bookings API
  slug: politecnico-di-torino-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-bookings-api-openapi.yml
- filename: politecnico-di-torino-courses-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Courses API
  slug: politecnico-di-torino-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-courses-api-openapi.yml
- filename: politecnico-di-torino-esc-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Esc API
  slug: politecnico-di-torino-esc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-esc-api-openapi.yml
- filename: politecnico-di-torino-exams-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Exams API
  slug: politecnico-di-torino-exams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-exams-api-openapi.yml
- filename: politecnico-di-torino-job-offers-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Job offers API
  slug: politecnico-di-torino-job-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-job-offers-api-openapi.yml
- filename: politecnico-di-torino-lectures-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Lectures API
  slug: politecnico-di-torino-lectures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-lectures-api-openapi.yml
- filename: politecnico-di-torino-news-api-openapi.yml
  format: yaml
  label: Politecnico di Torino News API
  slug: politecnico-di-torino-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-news-api-openapi.yml
- filename: politecnico-di-torino-offering-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Offering API
  slug: politecnico-di-torino-offering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-offering-api-openapi.yml
- filename: politecnico-di-torino-people-api-openapi.yml
  format: yaml
  label: Politecnico di Torino People API
  slug: politecnico-di-torino-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-people-api-openapi.yml
- filename: politecnico-di-torino-places-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Places API
  slug: politecnico-di-torino-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-places-api-openapi.yml
- filename: politecnico-di-torino-student-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Student API
  slug: politecnico-di-torino-student-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-student-api-openapi.yml
- filename: politecnico-di-torino-surveys-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Surveys API
  slug: politecnico-di-torino-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-surveys-api-openapi.yml
- filename: politecnico-di-torino-tickets-api-openapi.yml
  format: yaml
  label: Politecnico di Torino Tickets API
  slug: politecnico-di-torino-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-tickets-api-openapi.yml
- filename: politecnico-di-torino-public-search-api-openapi.yml
  format: yaml
  label: PoliTO Public Search Web Services (people, departments, teachings, rooms)
  slug: public-search-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-public-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Politecnico Di Torino Authentication
name_suffix: Authentication
oauth_flows: []
overview: Politecnico di Torino secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Politecnico di Torino
provider_slug: politecnico-di-torino
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: Bearer
  sources:
  - openapi/politecnico-di-torino-faculty-api.yaml
  - openapi/politecnico-di-torino-students-api.yaml
  type: http
slug: politecnico-di-torino-authentication
source_filename: politecnico-di-torino-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/politecnico-di-torino-faculty-api.yaml, openapi/politecnico-di-torino-students-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: Bearer\n  sources:\n  - openapi/politecnico-di-torino-faculty-api.yaml\n  - openapi/politecnico-di-torino-students-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/authentication/politecnico-di-torino-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Technical University
- Italy
- Course Catalog
- Research Data
- Identity Federation
- Open Data
- Mobile
- OpenAPI
---
