---
api_key_in: []
api_specs:
- filename: cardiff-courses-api-openapi.yml
  format: yaml
  label: Cardiff University Courses API
  slug: cardiff-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses-api-openapi.yml
- filename: cardiff-clearing-adjustments-api-openapi.yml
  format: yaml
  label: Cardiff University Clearing Adjustments API
  slug: cardiff-clearing-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-clearing-adjustments-api-openapi.yml
- filename: cardiff-groups-api-openapi.yml
  format: yaml
  label: Cardiff University Groups API
  slug: cardiff-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-groups-api-openapi.yml
- filename: cardiff-modules-api-openapi.yml
  format: yaml
  label: Cardiff University Modules API
  slug: cardiff-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules-api-openapi.yml
- filename: cardiff-assessments-api-openapi.yml
  format: yaml
  label: Cardiff University Assessments API
  slug: cardiff-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-assessments-api-openapi.yml
- filename: cardiff-occurrences-api-openapi.yml
  format: yaml
  label: Cardiff University Occurrences API
  slug: cardiff-occurrences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-occurrences-api-openapi.yml
- filename: cardiff-rollover-api-openapi.yml
  format: yaml
  label: Cardiff University Rollover API
  slug: cardiff-rollover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-rollover-api-openapi.yml
- filename: cardiff-schools-api-openapi.yml
  format: yaml
  label: Cardiff University Schools API
  slug: cardiff-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-schools-api-openapi.yml
- filename: cardiff-subjects-api-openapi.yml
  format: yaml
  label: Cardiff University Subjects API
  slug: cardiff-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-subjects-api-openapi.yml
- filename: cardiff-levels-api-openapi.yml
  format: yaml
  label: Cardiff University Levels API
  slug: cardiff-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-levels-api-openapi.yml
- filename: cardiff-semesters-api-openapi.yml
  format: yaml
  label: Cardiff University Semesters API
  slug: cardiff-semesters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-semesters-api-openapi.yml
- filename: cardiff-qualifications-api-openapi.yml
  format: yaml
  label: Cardiff University Qualifications API
  slug: cardiff-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-qualifications-api-openapi.yml
- filename: cardiff-years-api-openapi.yml
  format: yaml
  label: Cardiff University Years API
  slug: cardiff-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-years-api-openapi.yml
- filename: cardiff-publications-api-openapi.yml
  format: yaml
  label: Cardiff University Publications API
  slug: cardiff-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications-api-openapi.yml
- filename: cardiff-default-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Default API
  slug: cardiff-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-default-api-openapi.yml
- filename: cardiff-test-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Test API
  slug: cardiff-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-test-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cardiff Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Cardiff University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Cardiff University
provider_slug: cardiff
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
    scopes: 1
  name: default
  sources:
  - openapi/cardiff-courses.yaml
  - openapi/cardiff-echo.yaml
  - openapi/cardiff-lookups.yaml
  - openapi/cardiff-modules.yaml
  - openapi/cardiff-publications.yaml
  type: oauth2
slug: cardiff-authentication
source_filename: cardiff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cardiff-courses.yaml, openapi/cardiff-echo.yaml, openapi/cardiff-lookups.yaml,\n  openapi/cardiff-modules.yaml, openapi/cardiff-publications.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: default\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\n    scopes: 1\n  sources:\n  - openapi/cardiff-courses.yaml\n  - openapi/cardiff-echo.yaml\n  - openapi/cardiff-lookups.yaml\n  - openapi/cardiff-modules.yaml\n  - openapi/cardiff-publications.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/authentication/cardiff-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Public Research University
- United Kingdom
- Wales
- Russell Group
- Open Data
- Course Catalog
- Research Repository
- Identity Federation
- Research Computing
- Publications
---
