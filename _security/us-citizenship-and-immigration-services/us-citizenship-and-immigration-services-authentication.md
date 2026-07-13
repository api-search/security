---
api_key_in: []
api_specs:
- filename: uscis-case-status-api-openapi.yml
  format: yaml
  label: USCIS Case Status API
  slug: uscis-case-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-case-status-api-openapi.yml
- filename: uscis-foia-api-openapi.yml
  format: yaml
  label: USCIS FOIA Request and Status API
  slug: uscis-foia-request-and-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-foia-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Us Citizenship And Immigration Services Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: US Citizenship and Immigration Services secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: US Citizenship and Immigration Services
provider_slug: us-citizenship-and-immigration-services
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow. Obtain an access token from the USCIS token endpoint using your client_id and client_secret registered at developer.uscis.gov. Tokens expire after 1,800 seconds (30 minutes).
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api-int.uscis.gov/oauth/accesstoken
  name: OAuth2
  sources:
  - openapi/uscis-case-status-api-openapi.yml
  - openapi/uscis-foia-api-openapi.yml
  type: oauth2
slug: us-citizenship-and-immigration-services-authentication
source_filename: us-citizenship-and-immigration-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uscis-case-status-api-openapi.yml, openapi/uscis-foia-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-int.uscis.gov/oauth/accesstoken\n    scopes: 1\n  description: OAuth 2.0 Client Credentials flow. Obtain an access token from the USCIS token\n    endpoint using your client_id and client_secret registered at developer.uscis.gov. Tokens\n    expire after 1,800 seconds (30 minutes).\n  sources:\n  - openapi/uscis-case-status-api-openapi.yml\n  - openapi/uscis-foia-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/authentication/us-citizenship-and-immigration-services-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Federal Government
- Immigration
- Citizenship
- Case Status
- FOIA
---
