---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes supported by Appy Pie Automate as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Appypie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appy Pie LLP declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Appy Pie LLP
provider_slug: appypie
scheme_count: 3
schemes:
- evidence: Appy Pie Automate works with some of the most common authorization schemes such as Basic Auth, API key Auth, and OAuth V2.
  name: Basic Auth
  type: http-basic
- evidence: Appy Pie Automate works with some of the most common authorization schemes such as Basic Auth, API key Auth, and OAuth V2.
  name: API Key Auth
  type: apiKey
- authorize_url: https://accounts.google.com/o/oauth2/v2/auth
  evidence: For now, Appy Pie Automate supports OAuth V2 scheme to set up authentication for your app.
  flows:
  - authorization_code
  - client_credentials
  - refresh_token
  how_to_obtain: Configure client ID and secret in your app’s OAuth provider and paste the redirect URL provided by Appy Pie Automate.
  name: OAuth V2
  type: oauth2
slug: appypie-authentication
source_filename: appypie-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.appypie.com/docs/authentication
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.appypie.com/docs/authentication\nsources:\n- https://developer.appypie.com/docs/authentication\n- https://developer.appypie.com/docs/setting-up-authentication\n- https://developer.appypie.com/docs/setting-up-authentication#!authentication\n- https://developer.appypie.com/docs/setting-up-authentication#!select-your-authentication\ndescription: Authentication schemes supported by Appy Pie Automate as documented.\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: Appy Pie Automate works with some of the most common authorization schemes such as Basic Auth, API key Auth, and OAuth V2.\n- type: apiKey\n  name: API Key Auth\n  evidence: Appy Pie Automate works with some of the most common authorization schemes such as Basic Auth, API key Auth, and OAuth V2.\n- type: oauth2\n  name: OAuth V2\n  evidence: For now, Appy Pie Automate supports OAuth V2 scheme\
  \ to set up authentication for your app.\n  flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  authorize_url: https://accounts.google.com/o/oauth2/v2/auth\n  how_to_obtain: Configure client ID and secret in your app’s OAuth provider and paste the redirect URL provided by Appy Pie Automate.\ndocs: https://developer.appypie.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/appypie/authentication/appypie-authentication.yml
summary_line: 3 schemes
tags:
- No-Code
- Artificial Intelligence
- App Builder
- Mobile App
- Web App
---
