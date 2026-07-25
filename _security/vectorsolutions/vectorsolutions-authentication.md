---
api_key_in:
- header
api_specs:
- filename: vectorsolutions-courses-api-openapi.yml
  format: yaml
  label: Vector Solutions Courses API
  slug: vectorsolutions-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-courses-api-openapi.yml
- filename: vectorsolutions-credential-assignment-api-openapi.yml
  format: yaml
  label: Vector Solutions Credential Assignment API
  slug: vectorsolutions-credential-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-credential-assignment-api-openapi.yml
- filename: vectorsolutions-credential-categories-api-openapi.yml
  format: yaml
  label: Vector Solutions Credential Categories API
  slug: vectorsolutions-credential-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-credential-categories-api-openapi.yml
- filename: vectorsolutions-credentials-api-openapi.yml
  format: yaml
  label: Vector Solutions Credentials API
  slug: vectorsolutions-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-credentials-api-openapi.yml
- filename: vectorsolutions-feature-access-api-openapi.yml
  format: yaml
  label: Vector Solutions Feature Access API
  slug: vectorsolutions-feature-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-feature-access-api-openapi.yml
- filename: vectorsolutions-profile-categories-api-openapi.yml
  format: yaml
  label: Vector Solutions Profile Categories API
  slug: vectorsolutions-profile-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-profile-categories-api-openapi.yml
- filename: vectorsolutions-profile-group-assignment-api-openapi.yml
  format: yaml
  label: Vector Solutions Profile Group Assignment API
  slug: vectorsolutions-profile-group-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-profile-group-assignment-api-openapi.yml
- filename: vectorsolutions-profile-groups-api-openapi.yml
  format: yaml
  label: Vector Solutions Profile Groups API
  slug: vectorsolutions-profile-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-profile-groups-api-openapi.yml
- filename: vectorsolutions-sites-api-openapi.yml
  format: yaml
  label: Vector Solutions Sites API
  slug: vectorsolutions-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-sites-api-openapi.yml
- filename: vectorsolutions-supervisor-access-api-openapi.yml
  format: yaml
  label: Vector Solutions Supervisor Access API
  slug: vectorsolutions-supervisor-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-supervisor-access-api-openapi.yml
- filename: vectorsolutions-training-assignments-api-openapi.yml
  format: yaml
  label: Vector Solutions Training Assignments API
  slug: vectorsolutions-training-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-training-assignments-api-openapi.yml
- filename: vectorsolutions-user-emails-api-openapi.yml
  format: yaml
  label: Vector Solutions User Emails API
  slug: vectorsolutions-user-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-user-emails-api-openapi.yml
- filename: vectorsolutions-user-history-api-openapi.yml
  format: yaml
  label: Vector Solutions User History API
  slug: vectorsolutions-user-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-user-history-api-openapi.yml
- filename: vectorsolutions-users-api-openapi.yml
  format: yaml
  label: Vector Solutions Users API
  slug: vectorsolutions-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/openapi/vectorsolutions-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vectorsolutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vector Solutions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vector Solutions
provider_slug: vectorsolutions
scheme_count: 1
schemes:
- description: Customer-specific API token passed in the header of all requests over HTTPS. Requested from your TargetSolutions account manager; tokens can be read-only or feature-specific.
  in: header
  name: AccessToken
  parameter: AccessToken
  sources:
  - openapi/vectorsolutions-targetsolutions-openapi.yml
  type: apiKey
slug: vectorsolutions-authentication
source_filename: vectorsolutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/vectorsolutions-targetsolutions-openapi.yml\ndocs: https://developers.targetsolutions.com/worldoftargetsolutions\nnotes: TargetSolutions implements a basic-auth-over-HTTPS scheme requiring a customer-specific\n  API token in the AccessToken header of all requests. Tokens are requested from the\n  customer's account manager and can be issued read-only or feature-specific. Documented\n  on the developer portal getting-started page.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: AccessToken\n  description: Customer-specific API token passed in the header of all requests over HTTPS.\n    Requested from your TargetSolutions account manager; tokens can be read-only or feature-specific.\n  sources:\n  - openapi/vectorsolutions-targetsolutions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectorsolutions/refs/heads/main/authentication/vectorsolutions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Training
- Learning Management
- Compliance
- Public Safety
- Workforce Management
- EHS
- Education
---
