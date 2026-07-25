---
api_key_in: []
api_specs:
- filename: workday-business-processes-approvals-api-openapi.yml
  format: yaml
  label: Workday Business Processes Approvals API
  slug: workday-business-processes-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-approvals-api-openapi.yml
- filename: workday-business-processes-business-process-definitions-api-openapi.yml
  format: yaml
  label: Workday Business Processes Business Process Definitions API
  slug: workday-business-processes-business-process-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-definitions-api-openapi.yml
- filename: workday-business-processes-inbox-items-api-openapi.yml
  format: yaml
  label: Workday Business Processes Inbox Items API
  slug: workday-business-processes-inbox-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-inbox-items-api-openapi.yml
- filename: workday-business-processes-process-instances-api-openapi.yml
  format: yaml
  label: Workday Business Processes Process Instances API
  slug: workday-business-processes-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-process-instances-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Business Processes Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Workday Business Processes secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Workday Business Processes
provider_slug: workday-business-processes
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  sources:
  - openapi/workday-business-processes-openapi.yml
  type: oauth2
slug: workday-business-processes-authentication
source_filename: workday-business-processes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-business-processes-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n    scopes: 1\n  sources:\n  - openapi/workday-business-processes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/authentication/workday-business-processes-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
