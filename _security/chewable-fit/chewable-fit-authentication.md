---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Chewable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chewable declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chewable
provider_slug: chewable-fit
scheme_count: 1
schemes:
- applies_to: https://foodieapi.chewable.fit/mcp
  authorization_response_iss_parameter_supported: true
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  dynamic_client_registration: https://foodieapi.chewable.fit/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://foodieapi.chewable.fit/oauth/authorize
      scopes:
        foodie: Access to the user's Foodie recipes, meal plan and shopping list (scope name from metadata; description paraphrased from the connect guide)
      tokenUrl: https://foodieapi.chewable.fit/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  identity_provider: Sign in with Apple
  name: foodieOAuth
  pkce: S256
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: chewable-fit-authentication
source_filename: chewable-fit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://foodieapi.chewable.fit/.well-known/oauth-authorization-server\ndocs: https://foodie.chewable.fit/connect\nname: Chewable authentication\nnote: Read from the documented MCP host's published discovery documents (RFC 9728 protected-resource metadata at /.well-known/oauth-protected-resource, HTTP 200; RFC 8414 authorization-server metadata at /.well-known/oauth-authorization-server, HTTP 200). Authorization, token and registration endpoints were NOT called. Docs say sign-in is \"Continue with Apple\" with the same Apple ID as the Foodie app, and \"Accounts are made in the app only.\"\nschemes:\n- name: foodieOAuth\n  type: oauth2\n  applies_to: https://foodieapi.chewable.fit/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://foodieapi.chewable.fit/oauth/authorize\n      tokenUrl: https://foodieapi.chewable.fit/oauth/token\n      scopes:\n        foodie: Access to the user's Foodie recipes, meal plan and\
  \ shopping list (scope name from metadata; description paraphrased from the connect guide)\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  dynamic_client_registration: https://foodieapi.chewable.fit/oauth/register\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\n  bearer_methods: [header]\n  identity_provider: Sign in with Apple\n"
source_yaml_url: https://artifacts.apis.io/chewable-fit/authentication/chewable-fit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Mobile App
- iOS
- Recipes
- Meal Planning
- Fitness
- Strength Training
- Fashion
- Virtual Try-On
- Artificial Intelligence
- MCP
---
