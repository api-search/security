---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avocadoai-co-openapi.json
  format: json
  label: Avocado AI API
  slug: avocado-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avocadoai-co/openapi/avocadoai-co-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Avocado AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avocado AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Avocado AI
provider_slug: avocadoai-co
scheme_count: 2
schemes:
- description: Avocado API key (avk_) or OAuth access token.
  name: bearerAuth
  scheme: bearer
  type: http
- description: OAuth 2.1 authorization code with PKCE (S256). Public clients register dynamically at the registration endpoint.
  flows:
    authorizationCode:
      authorizationUrl: https://avocadoai.co/oauth/authorize
      scopes: {}
      tokenUrl: https://avocadoai.co/oauth/token
  name: oauth2
  type: oauth2
slug: avocadoai-co-authentication
source_filename: avocadoai-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://avocadoai.co/openapi.json\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: \"Avocado API key (avk_) or OAuth access token.\"\n  - name: oauth2\n    type: oauth2\n    description: \"OAuth 2.1 authorization code with PKCE (S256). Public clients register dynamically at the registration endpoint.\"\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://avocadoai.co/oauth/authorize\"\n        tokenUrl: \"https://avocadoai.co/oauth/token\"\n        scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/avocadoai-co/authentication/avocadoai-co-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Creative
- E-Commerce
- Image Generation
- Video Generation
---
