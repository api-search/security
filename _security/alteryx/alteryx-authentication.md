---
api_key_in: []
api_specs:
- filename: alteryx-collections-api-openapi.yml
  format: yaml
  label: Alteryx Collections API
  slug: alteryx-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-collections-api-openapi.yml
- filename: alteryx-credentials-api-openapi.yml
  format: yaml
  label: Alteryx Credentials API
  slug: alteryx-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-credentials-api-openapi.yml
- filename: alteryx-jobs-api-openapi.yml
  format: yaml
  label: Alteryx Jobs API
  slug: alteryx-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-jobs-api-openapi.yml
- filename: alteryx-schedules-api-openapi.yml
  format: yaml
  label: Alteryx Schedules API
  slug: alteryx-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-schedules-api-openapi.yml
- filename: alteryx-users-api-openapi.yml
  format: yaml
  label: Alteryx Users API
  slug: alteryx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-users-api-openapi.yml
- filename: alteryx-workflows-api-openapi.yml
  format: yaml
  label: Alteryx Workflows API
  slug: alteryx-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-workflows-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Alteryx Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alteryx secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alteryx
provider_slug: alteryx
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  sources:
  - openapi/alteryx-server-api-v3.yml
  type: oauth2
slug: alteryx-authentication
source_filename: alteryx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alteryx-server-api-v3.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\n  sources:\n  - openapi/alteryx-server-api-v3.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/authentication/alteryx-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
---
