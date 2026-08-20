---
api_key_in: []
api_specs:
- filename: submittable-assignments-api-openapi.yml
  format: yaml
  label: Submittable Assignments API
  slug: submittable-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-assignments-api-openapi.yml
- filename: submittable-entries-api-openapi.yml
  format: yaml
  label: Submittable Entries API
  slug: submittable-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-entries-api-openapi.yml
- filename: submittable-funds-api-openapi.yml
  format: yaml
  label: Submittable Funds API
  slug: submittable-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-funds-api-openapi.yml
- filename: submittable-labels-api-openapi.yml
  format: yaml
  label: Submittable Labels API
  slug: submittable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-labels-api-openapi.yml
- filename: submittable-messaging-api-openapi.yml
  format: yaml
  label: Submittable Messaging API
  slug: submittable-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-messaging-api-openapi.yml
- filename: submittable-payments-api-openapi.yml
  format: yaml
  label: Submittable Payments API
  slug: submittable-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-payments-api-openapi.yml
- filename: submittable-projects-api-openapi.yml
  format: yaml
  label: Submittable Projects API
  slug: submittable-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-projects-api-openapi.yml
- filename: submittable-submissions-api-openapi.yml
  format: yaml
  label: Submittable Submissions API
  slug: submittable-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-submissions-api-openapi.yml
- filename: submittable-teams-api-openapi.yml
  format: yaml
  label: Submittable Teams API
  slug: submittable-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-teams-api-openapi.yml
- filename: submittable-users-api-openapi.yml
  format: yaml
  label: Submittable Users API
  slug: submittable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-users-api-openapi.yml
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
- Application
- Forms
- Non-Profit
- Corporate Social Responsibility
- Workflows
---
