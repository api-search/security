---
api_key_in: []
api_specs:
- filename: medidata-audit-api-openapi.yml
  format: yaml
  label: medidata Audit API
  slug: medidata-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-audit-api-openapi.yml
- filename: medidata-clinical-data-api-openapi.yml
  format: yaml
  label: medidata Clinical Data API
  slug: medidata-clinical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-clinical-data-api-openapi.yml
- filename: medidata-queries-api-openapi.yml
  format: yaml
  label: medidata Queries API
  slug: medidata-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-queries-api-openapi.yml
- filename: medidata-sites-api-openapi.yml
  format: yaml
  label: medidata Sites API
  slug: medidata-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-sites-api-openapi.yml
- filename: medidata-studies-api-openapi.yml
  format: yaml
  label: medidata Studies API
  slug: medidata-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-studies-api-openapi.yml
- filename: medidata-subjects-api-openapi.yml
  format: yaml
  label: medidata Subjects API
  slug: medidata-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-subjects-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Medidata Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: medidata secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: medidata
provider_slug: medidata
scheme_count: 2
schemes:
- description: Medidata Rave username and password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/medidata-rave-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://identity.medidata.com/connect/token
  name: OAuth2
  sources:
  - openapi/medidata-rave-openapi.yml
  type: oauth2
slug: medidata-authentication
source_filename: medidata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/medidata-rave-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Medidata Rave username and password\n  sources:\n  - openapi/medidata-rave-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.medidata.com/connect/token\n    scopes: 2\n  sources:\n  - openapi/medidata-rave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/authentication/medidata-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---
