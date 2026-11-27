---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-apps-script-processes-api-openapi.yml
  format: yaml
  label: Google Apps Script Processes API
  slug: google-apps-script-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-apps-script/openapi/google-apps-script-processes-api-openapi.yml
- filename: google-apps-script-projects-api-openapi.yml
  format: yaml
  label: Google Apps Script Projects API
  slug: google-apps-script-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-apps-script/openapi/google-apps-script-projects-api-openapi.yml
- filename: google-apps-script-scripts-api-openapi.yml
  format: yaml
  label: Google Apps Script Scripts API
  slug: google-apps-script-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-apps-script/openapi/google-apps-script-scripts-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Google Apps Script Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Apps Script declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Google Apps Script
provider_slug: google-apps-script
scheme_count: 1
schemes:
- evidence: Provide a properly scoped OAuth token for the execution.
  flows:
    authorizationCode:
      authorizationUrl: https://accounts.google.com/o/oauth2/auth
      tokenUrl: https://oauth2.googleapis.com/token
  scopes_ref: scopes/google-apps-script-scopes.yml
  type: oauth2
slug: google-apps-script-authentication
source_filename: google-apps-script-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Google Apps Script authentication\ngenerated: '2026-11-11'\nmethod: searched\nsource: https://developers.google.com/apps-script/api/how-tos/execute\ndocs: https://developers.google.com/apps-script/api/how-tos/execute\nschemes:\n- type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://accounts.google.com/o/oauth2/auth\n      tokenUrl: https://oauth2.googleapis.com/token\n  scopes_ref: scopes/google-apps-script-scopes.yml\n  evidence: Provide a properly scoped OAuth token for the execution.\nnotes:\n- 'Warning: The Apps Script API doesn''t work with service accounts .'\n"
source_yaml_url: https://artifacts.apis.io/google-apps-script/authentication/google-apps-script-authentication.yml
summary_line: 1 scheme
tags:
- Apps Script
- Automation
- Deployment
- Google
- Google Workspace
- Scripting
---
