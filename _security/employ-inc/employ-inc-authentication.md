---
anonymous_access: false
api_key_in: []
api_specs:
- filename: employ-inc-status-api-openapi.yml
  format: yaml
  label: Employ Inc Status API
  slug: employ-inc-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employ-inc/refs/heads/main/openapi/employ-inc-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Employ Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Employ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Employ
provider_slug: employ-inc
scheme_count: 1
schemes:
- description: 'WordPress application password (HTTP Basic). Authorization endpoint: https://www.employinc.com/wp-admin/authorize-application.php. Declared by the site''s own discovery document under authentication.application-passwords.'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/employ-inc-content-api-openapi.yml
  - openapi/employ-inc-tec-events-rest-api-openapi.json
  type: http
slug: employ-inc-authentication
source_filename: employ-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: derived\nsource: openapi/employ-inc-content-api-openapi.yml, openapi/employ-inc-tec-events-rest-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress application password (HTTP Basic). Authorization endpoint: https://www.employinc.com/wp-admin/authorize-application.php.\n    Declared by the site''s own discovery document under authentication.application-passwords.'\n  sources:\n  - openapi/employ-inc-content-api-openapi.yml\n  - openapi/employ-inc-tec-events-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employ-inc/refs/heads/main/authentication/employ-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Applicant Tracking
- Hiring
- Content
- Event
- Status
---
