---
api_key_in: []
api_specs:
- filename: phenom-applicants-api-openapi.yml
  format: yaml
  label: Phenom Applicants API
  slug: phenom-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-applicants-api-openapi.yml
- filename: phenom-applications-api-openapi.yml
  format: yaml
  label: Phenom Applications API
  slug: phenom-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-applications-api-openapi.yml
- filename: phenom-candidates-api-openapi.yml
  format: yaml
  label: Phenom Candidates API
  slug: phenom-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-candidates-api-openapi.yml
- filename: phenom-jobs-api-openapi.yml
  format: yaml
  label: Phenom Jobs API
  slug: phenom-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-jobs-api-openapi.yml
- filename: phenom-onboarding-api-openapi.yml
  format: yaml
  label: Phenom Onboarding API
  slug: phenom-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-onboarding-api-openapi.yml
- filename: phenom-parsers-api-openapi.yml
  format: yaml
  label: Phenom Parsers API
  slug: phenom-parsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-parsers-api-openapi.yml
- filename: phenom-prediction-api-openapi.yml
  format: yaml
  label: Phenom Prediction API
  slug: phenom-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-prediction-api-openapi.yml
- filename: phenom-tags-api-openapi.yml
  format: yaml
  label: Phenom Tags API
  slug: phenom-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-tags-api-openapi.yml
- filename: phenom-user-management-api-openapi.yml
  format: yaml
  label: Phenom User Management API
  slug: phenom-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/openapi/phenom-user-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Phenom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phenom secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phenom
provider_slug: phenom
scheme_count: 1
schemes:
- description: 'Every Phenom platform operation requires a bearer token supplied in the Authorization request header (documented as `Authorization: <token>`). Tokens/credentials are provisioned per tenant via the Phenom Developer Portal.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/phenom-platform-openapi.yml
  type: http
slug: phenom-authentication
source_filename: phenom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/phenom-platform-openapi.yml\ndocs: https://developer.phenom.com/getStarted\nsummary:\n  types:\n  - http\n  scheme: bearer\n  context_headers:\n  - x-ph-userId\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    Every Phenom platform operation requires a bearer token supplied in the\n    Authorization request header (documented as `Authorization: <token>`).\n    Tokens/credentials are provisioned per tenant via the Phenom Developer Portal.\n  sources:\n  - openapi/phenom-platform-openapi.yml\ncontext_headers:\n- name: x-ph-userId\n  required_on:\n  - Candidates\n  - Applicants\n  - Tags\n  description: >-\n    Phenom user identifier that scopes the request to an acting user; required on\n    candidate, applicant and tag operations (header casing varies: x-ph-userId / x-ph-userid).\nnotes: >-\n  User Management APIs implement the SCIM 2.0 protocol\
  \ for provisioning users and groups.\n  No OAuth2 authorization/token endpoints are documented; auth is bearer-token based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phenom/refs/heads/main/authentication/phenom-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Hr Tech
- Talent Experience
- Recruiting
- Applicant Tracking
- Candidate Experience
- Onboarding
- SCIM
- Resume Parsing
- Skills
- Artificial Intelligence
---
