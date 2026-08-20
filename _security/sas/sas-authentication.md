---
api_key_in: []
api_specs:
- filename: sas-businessrules-api-openapi.yml
  format: yaml
  label: SAS Institute BusinessRules API
  slug: sas-businessrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-businessrules-api-openapi.yml
- filename: sas-cas-api-openapi.yml
  format: yaml
  label: SAS Institute CAS API
  slug: sas-cas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-cas-api-openapi.yml
- filename: sas-decisions-api-openapi.yml
  format: yaml
  label: SAS Institute Decisions API
  slug: sas-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-decisions-api-openapi.yml
- filename: sas-files-api-openapi.yml
  format: yaml
  label: SAS Institute Files API
  slug: sas-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-files-api-openapi.yml
- filename: sas-folders-api-openapi.yml
  format: yaml
  label: SAS Institute Folders API
  slug: sas-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-folders-api-openapi.yml
- filename: sas-identities-api-openapi.yml
  format: yaml
  label: SAS Institute Identities API
  slug: sas-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-identities-api-openapi.yml
- filename: sas-jobs-api-openapi.yml
  format: yaml
  label: SAS Institute Jobs API
  slug: sas-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-jobs-api-openapi.yml
- filename: sas-logon-api-openapi.yml
  format: yaml
  label: SAS Institute Logon API
  slug: sas-logon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-logon-api-openapi.yml
- filename: sas-models-api-openapi.yml
  format: yaml
  label: SAS Institute Models API
  slug: sas-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-models-api-openapi.yml
- filename: sas-reports-api-openapi.yml
  format: yaml
  label: SAS Institute Reports API
  slug: sas-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-reports-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sas Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: SAS Institute secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: SAS Institute
provider_slug: sas
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 1
    tokenUrl: /SASLogon/oauth/token
  name: oauth2
  sources:
  - openapi/sas-viya-rest-api-openapi.yml
  type: oauth2
slug: sas-authentication
source_filename: sas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sas-viya-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /SASLogon/oauth/token\n    scopes: 1\n  sources:\n  - openapi/sas-viya-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/authentication/sas-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Data Management
- Artificial Intelligence
- Machine-Learning
- Software
---
