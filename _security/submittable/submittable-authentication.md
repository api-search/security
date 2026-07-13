---
api_key_in: []
api_specs:
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Submissions API
  slug: submittable-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Entries API
  slug: submittable-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Projects and Forms API
  slug: submittable-projects-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Users (Submitters) API
  slug: submittable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Teams and Reviews API
  slug: submittable-teams-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Labels API
  slug: submittable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Funds and Payments API
  slug: submittable-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Submittable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Submittable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Submittable
provider_slug: submittable
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. Send your account access token as the password portion of the Basic Auth header (the username may be left blank or set to your account email, per Submittable's documentation).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/submittable-openapi.yml
  type: http
slug: submittable-authentication
source_filename: submittable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/submittable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Send your account access token as the password portion\n    of the Basic Auth header (the username may be left blank or set to your account email, per\n    Submittable's documentation).\n  sources:\n  - openapi/submittable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/authentication/submittable-authentication.yml
summary_line: http · 1 scheme
tags:
- Submission Management
- Grants Management
- Applications
- Forms
- Nonprofit
- Corporate Social Responsibility
- Workflow
---
