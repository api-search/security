---
api_key_in: []
api_specs:
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Interviews API
  slug: spark-hire-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Interview Questions API
  slug: spark-hire-interview-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Jobs API
  slug: spark-hire-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Users API
  slug: spark-hire-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Webhooks API
  slug: spark-hire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Account and Plan API
  slug: spark-hire-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spark Hire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spark Hire secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spark Hire
provider_slug: spark-hire
scheme_count: 1
schemes:
- description: HTTP Basic authentication. The username is your Spark Hire API key; the password is ignored. Keys are scoped to a user and respect that user's permission level.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/spark-hire-openapi.yml
  type: http
slug: spark-hire-authentication
source_filename: spark-hire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spark-hire-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. The username is your Spark Hire API key; the password\n    is ignored. Keys are scoped to a user and respect that user's permission level.\n  sources:\n  - openapi/spark-hire-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/authentication/spark-hire-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Interviewing
- Recruiting
- Hiring
- HR Tech
- Talent Assessment
- ATS
---
