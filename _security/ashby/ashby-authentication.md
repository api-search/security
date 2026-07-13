---
api_key_in:
- header
api_specs:
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Candidates API
  slug: ashby-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Applications API
  slug: ashby-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Jobs API
  slug: ashby-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Openings API
  slug: ashby-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Job Postings API
  slug: ashby-job-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Offers API
  slug: ashby-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Interviews API
  slug: ashby-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Interview Schedules API
  slug: ashby-interview-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Feedback API
  slug: ashby-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Feedback Form Definitions API
  slug: ashby-feedback-form-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Hiring Team API
  slug: ashby-hiring-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Archive Reasons API
  slug: ashby-archive-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Sources API
  slug: ashby-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Surveys API
  slug: ashby-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Locations API
  slug: ashby-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Departments API
  slug: ashby-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Custom Fields API
  slug: ashby-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Users API
  slug: ashby-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Webhooks API
  slug: ashby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Partner Job Feed
  slug: ashby-job-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
- filename: ashby-api-openapi.json
  format: json
  label: Ashby Careers Page API
  slug: ashby-careers-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/openapi/ashby-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ashby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ashby secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ashby
provider_slug: ashby
scheme_count: 2
schemes:
- description: "Use HTTP Basic Auth to authenticate with our API. You must send your API key with every request. \nPut your API key as the basic auth username and leave the password blank."
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/ashby-api-openapi.json
  - openapi/ashby-assessments-partner-openapi.json
  type: http
- description: '[Optional] If you provide a secret token when configuring your webhook, this will be used to create a digest of the JSON payload sent with each webhook request.

    The digest will be included in the request under the `Ashby-Signature` http header.


    It will look like this:

    `Ashby-Signature: sha256=f3124911d2956f10aa3a49c43a88bdf13bba846e94f0ae2bd7c034f90239bd04`


    The part before the = indicates the al'
  in: header
  name: WebhookSignature
  parameter: Ashby-Signature
  sources:
  - openapi/ashby-api-openapi.json
  type: apiKey
slug: ashby-authentication
source_filename: ashby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ashby-api-openapi.json, openapi/ashby-assessments-partner-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: \"Use HTTP Basic Auth to authenticate with our API. You must send your API key\\\n    \\ with every request. \\nPut your API key as the basic auth username and leave the password\\\n    \\ blank.\"\n  sources:\n  - openapi/ashby-api-openapi.json\n  - openapi/ashby-assessments-partner-openapi.json\n- name: WebhookSignature\n  type: apiKey\n  in: header\n  parameter: Ashby-Signature\n  description: |-\n    [Optional] If you provide a secret token when configuring your webhook, this will be used to create a digest of the JSON payload sent with each webhook request.\n    The digest will be included in the request under the `Ashby-Signature` http header.\n\n    It will look like this:\n    `Ashby-Signature: sha256=f3124911d2956f10aa3a49c43a88bdf13bba846e94f0ae2bd7c034f90239bd04`\n\
  \n    The part before the = indicates the al\n  sources:\n  - openapi/ashby-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ashby/refs/heads/main/authentication/ashby-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- HR
- ATS
- Recruiting
- Analytics
- Sourcing
- Scheduling
---
