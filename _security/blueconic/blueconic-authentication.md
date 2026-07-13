---
api_key_in: []
api_specs:
- filename: rest.apidoc.blueconic.com
  format: yaml
  label: BlueConic REST API v2
  slug: blueconic-rest-api-v2
  spec_type: OpenAPI
  url: https://rest.apidoc.blueconic.com
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Blueconic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: BlueConic secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: BlueConic
provider_slug: blueconic
scheme_count: 1
schemes:
- description: Authenticates a registered OAuth 2.0 client. The Authorization code flow and Client credentials flow are supported. Make sure to select the correct flow based on which flow the registered client supports. The client id and client secret can be found in BlueConic by opening the registered client under *Settings* > *Access management* > *Applications*.<br/>**NOTE:** When using the Authorization code
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /rest/v2/oauth/token
  - authorizationUrl: /rest/v2/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /rest/v2/oauth/token
  name: oauth2
  sources:
  - openapi/blueconic-rest-api-v2-openapi.yml
  type: oauth2
slug: blueconic-authentication
source_filename: blueconic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blueconic-rest-api-v2-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /rest/v2/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /rest/v2/oauth/authorize\n    tokenUrl: /rest/v2/oauth/token\n    scopes: 0\n  description: Authenticates a registered OAuth 2.0 client. The Authorization code flow and\n    Client credentials flow are supported. Make sure to select the correct flow based on which\n    flow the registered client supports. The client id and client secret can be found in BlueConic\n    by opening the registered client under *Settings* > *Access management* > *Applications*.<br/>**NOTE:**\n    When using the Authorization code\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueconic/refs/heads/main/authentication/blueconic-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Customer Data Platform
- CDP
- Customer Profiles
- Segments
- Data Activation
- First-Party Data
- Lifecycle Stages
- Connections
- Privacy
---
