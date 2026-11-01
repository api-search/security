---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orchesty-2.0-openapi-generated.yml
  format: yaml
  label: Orchesty.io 2.0 API
  slug: 2.0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchesty/openapi/_ae-authored/orchesty-2.0-openapi-generated.yml
- filename: orchesty-3.0-openapi-generated.yml
  format: yaml
  label: Orchesty.io 3.0 API
  slug: 3.0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchesty/openapi/_ae-authored/orchesty-3.0-openapi-generated.yml
auth_types: []
description: Authentication methods supported by Orchesty applications
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Orchesty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orchesty.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Orchesty.io
provider_slug: orchesty
scheme_count: 2
schemes:
- evidence: 'Authorization'' : `Bearer ${ apiKey }`'
  header: Authorization
  how_to_obtain: Provided as a static API key in the Application's Authorization form
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://auth.wflow.com/oauth/authorize
  evidence: 'public getAuthUrl () : string { return ''https://auth.wflow.com/oauth/authorize'' ; }'
  flows:
  - authorization_code
  how_to_obtain: User authorizes via the Admin UI which redirects to the provider's authorization endpoint
  name: OAuth2
  scopes:
  - read_invoices
  - write_invoices
  token_url: https://auth.wflow.com/oauth/token
  type: oauth2
slug: orchesty-authentication
source_filename: orchesty-authentication.yml
source_heading: Authentication Profile
source_url: https://orchesty.io/docs/3.0/development/authentication-and-settings/authentication-and-settings
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://orchesty.io/docs/3.0/development/authentication-and-settings/authentication-and-settings\nsources:\n- https://orchesty.io/docs/3.0/development/authentication-and-settings/authentication-and-settings\n- https://orchesty.io/docs/3.0/development/authentication-and-settings/modules\n- https://orchesty.io/docs/3.0/development/authentication-and-settings/basic-application\n- https://orchesty.io/docs/3.0/development/authentication-and-settings/oauth2-application\ndescription: Authentication methods supported by Orchesty applications\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization'' : `Bearer ${ apiKey }`'\n  location: header\n  header: Authorization\n  how_to_obtain: Provided as a static API key in the Application's Authorization form\n- type: oauth2\n  name: OAuth2\n  evidence: 'public getAuthUrl () : string { return ''https://auth.wflow.com/oauth/authorize''\
  \ ; }'\n  flows:\n  - authorization_code\n  token_url: https://auth.wflow.com/oauth/token\n  authorize_url: https://auth.wflow.com/oauth/authorize\n  scopes:\n  - read_invoices\n  - write_invoices\n  how_to_obtain: User authorizes via the Admin UI which redirects to the provider's authorization endpoint\ndocs: https://orchesty.io/docs/3.0/development/authentication-and-settings/authentication-and-settings\n"
source_yaml_url: https://artifacts.apis.io/orchesty/authentication/orchesty-authentication.yml
summary_line: 2 schemes
tags:
- Integration
- Platform
- Automation
- Artificial Intelligence
- Open Source
---
