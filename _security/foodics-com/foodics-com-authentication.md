---
anonymous_access: false
api_key_in: []
auth_types: []
description: OAuth2 authorization code flow
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Foodics Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alwans declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Alwans
provider_slug: foodics-com
scheme_count: 1
schemes:
- authorize_url: https://console.foodics.com/authorize?client_id={your_client_id}&state={random_string}
  evidence: Initiate OAuth flow through the below link, which will represent the Install button for your application under the Marketplace module as shown on the below screenshot.
  flows:
  - authorization_code
  how_to_obtain: User authorizes the app via the Foodics Authorization server, which redirects back with an authorization code that the app exchanges for an access token.
  name: OAuth2
  type: oauth2
slug: foodics-com-authentication
source_filename: foodics-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.foodics.com/guides/partnership_authentication_process
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.foodics.com/guides/partnership_authentication_process\nsources:\n- https://developers.foodics.com/guides/partnership_authentication_process\ndescription: OAuth2 authorization code flow\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: Initiate OAuth flow through the below link, which will represent the Install button for your application under the Marketplace module\n    as shown on the below screenshot.\n  flows:\n  - authorization_code\n  authorize_url: https://console.foodics.com/authorize?client_id={your_client_id}&state={random_string}\n  how_to_obtain: User authorizes the app via the Foodics Authorization server, which redirects back with an authorization code that the app exchanges\n    for an access token.\ndocs: https://developers.foodics.com/guides/partnership_authentication_process\n"
source_yaml_url: https://artifacts.apis.io/foodics-com/authentication/foodics-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Restaurant
- SaaS
- API
- Cloud
---
