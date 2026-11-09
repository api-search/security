---
anonymous_access: false
api_key_in: []
api_specs:
- filename: beyourcover-com-account-api-openapi.yml
  format: yaml
  label: BeYourCover Account API
  slug: beyourcover-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-account-api-openapi.yml
- filename: beyourcover-com-books-api-openapi.yml
  format: yaml
  label: BeYourCover Books API
  slug: beyourcover-com-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-books-api-openapi.yml
- filename: beyourcover-com-clients-api-openapi.yml
  format: yaml
  label: BeYourCover Clients API
  slug: beyourcover-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-clients-api-openapi.yml
- filename: beyourcover-com-covers-api-openapi.yml
  format: yaml
  label: BeYourCover Covers API
  slug: beyourcover-com-covers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-covers-api-openapi.yml
- filename: beyourcover-com-jobs-api-openapi.yml
  format: yaml
  label: BeYourCover Jobs API
  slug: beyourcover-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-jobs-api-openapi.yml
- filename: beyourcover-com-service-api-openapi.yml
  format: yaml
  label: BeYourCover Service API
  slug: beyourcover-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-service-api-openapi.yml
- filename: beyourcover-com-templates-api-openapi.yml
  format: yaml
  label: BeYourCover Templates API
  slug: beyourcover-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-templates-api-openapi.yml
- filename: beyourcover-com-wraps-api-openapi.yml
  format: yaml
  label: BeYourCover Wraps API
  slug: beyourcover-com-wraps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beyourcover-com/openapi/beyourcover-com-wraps-api-openapi.yml
auth_types: []
description: Authentication methods for BeYourCover APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Beyourcover Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BeYourCover declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BeYourCover
provider_slug: beyourcover-com
scheme_count: 2
schemes:
- evidence: OAuth 2.1 authorization code + PKCE — MCP endpoint only
  flows:
  - authorization_code
  how_to_obtain: Register a client at the registration_endpoint (dynamic client registration) and run the authorization code flow with PKCE, then exchange the code at the token_endpoint for an access token.
  name: OAuth 2.1 authorization code + PKCE
  scopes:
  - openid
  - email
  - offline_access
  type: oauth2
- evidence: Send it in the `Authorization` header. This is the only accepted method — no query parameter, no request-body field.
  header: Authorization
  how_to_obtain: Subscribe to an API plan at https://beyourcover.com/for-publishers and create the key in the account dashboard at https://beyourcover.com/account-dashboard.
  location: header
  name: Partner API key
  type: apiKey
slug: beyourcover-com-authentication
source_filename: beyourcover-com-authentication.yml
source_heading: Authentication Profile
source_url: https://beyourcover.com/auth.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://beyourcover.com/auth.md\nsources:\n- https://beyourcover.com/auth.md\n- https://beyourcover.com/docs/getting-started.md\n- https://beyourcover.com/docs/getting-started\ndescription: Authentication methods for BeYourCover APIs\nschemes:\n- type: oauth2\n  name: OAuth 2.1 authorization code + PKCE\n  evidence: OAuth 2.1 authorization code + PKCE — MCP endpoint only\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - email\n  - offline_access\n  how_to_obtain: Register a client at the registration_endpoint (dynamic client registration) and run the authorization code flow with PKCE, then\n    exchange the code at the token_endpoint for an access token.\n- type: apiKey\n  name: Partner API key\n  evidence: Send it in the `Authorization` header. This is the only accepted method — no query parameter, no request-body field.\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: Subscribe to an API plan at https://beyourcover.com/for-publishers and create the key in the account dashboard at https://beyourcover.com/account-dashboard.\ndocs: https://beyourcover.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/beyourcover-com/authentication/beyourcover-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- BookCover
- Design
- Publishing
---
