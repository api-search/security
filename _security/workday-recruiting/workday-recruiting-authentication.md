---
api_key_in: []
api_specs:
- filename: workday-recruiting-agentdefinition-api-openapi.yml
  format: yaml
  label: Workday Recruiting agentDefinition API
  slug: workday-recruiting-agentdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-agentdefinition-api-openapi.yml
- filename: workday-recruiting-applicants-api-openapi.yml
  format: yaml
  label: Workday Recruiting Applicants API
  slug: workday-recruiting-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-applicants-api-openapi.yml
- filename: workday-recruiting-background-checks-api-openapi.yml
  format: yaml
  label: Workday Recruiting Background Checks API
  slug: workday-recruiting-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-background-checks-api-openapi.yml
- filename: workday-recruiting-candidates-api-openapi.yml
  format: yaml
  label: Workday Recruiting Candidates API
  slug: workday-recruiting-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-candidates-api-openapi.yml
- filename: workday-recruiting-configuration-api-openapi.yml
  format: yaml
  label: Workday Recruiting Configuration API
  slug: workday-recruiting-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-configuration-api-openapi.yml
- filename: workday-recruiting-evergreen-requisitions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Evergreen Requisitions API
  slug: workday-recruiting-evergreen-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-evergreen-requisitions-api-openapi.yml
- filename: workday-recruiting-interviews-api-openapi.yml
  format: yaml
  label: Workday Recruiting Interviews API
  slug: workday-recruiting-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-interviews-api-openapi.yml
- filename: workday-recruiting-job-applications-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Applications API
  slug: workday-recruiting-job-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-applications-api-openapi.yml
- filename: workday-recruiting-job-postings-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Postings API
  slug: workday-recruiting-job-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-postings-api-openapi.yml
- filename: workday-recruiting-job-requisitions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Requisitions API
  slug: workday-recruiting-job-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-requisitions-api-openapi.yml
- filename: workday-recruiting-positions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Positions API
  slug: workday-recruiting-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-positions-api-openapi.yml
- filename: workday-recruiting-recruiting-agencies-api-openapi.yml
  format: yaml
  label: Workday Recruiting Recruiting Agencies API
  slug: workday-recruiting-recruiting-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-recruiting-agencies-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Recruiting Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Recruiting secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Recruiting
provider_slug: workday-recruiting
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting scopes, and obtain access tokens.
  flows:
  - authorizationUrl: https://{tenant}.workday.com/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token
  name: oauth2
  sources:
  - openapi/workday-recruiting-rest-api-openapi.yml
  type: oauth2
slug: workday-recruiting-authentication
source_filename: workday-recruiting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-recruiting-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.workday.com/authorize\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token\n    scopes: 2\n  description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting\n    scopes, and obtain access tokens.\n  sources:\n  - openapi/workday-recruiting-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/authentication/workday-recruiting-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HCM
- Human Resources
- Recruiting
- SaaS
- Talent Acquisition
---
