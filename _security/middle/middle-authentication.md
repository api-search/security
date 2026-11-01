---
anonymous_access: false
api_key_in: []
api_specs:
- filename: middle-openapi-generated.yml
  format: yaml
  label: Middle API
  slug: middle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/middle/openapi/_ae-authored/middle-openapi-generated.yml
auth_types: []
description: Authentication methods supported by Middle as described in the documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Middle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Middle declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Middle
provider_slug: middle
scheme_count: 3
schemes:
- evidence: This authentication is best suited for non-OAuth authentications where the system you are integrating with requires an individual username/password, business ID, key, or a predetermined token for each connection.
  name: Custom fields
  type: other
- evidence: The password grant flow is made to support the OAuth2.0 Password Grant flow of the same name.
  flows:
  - password_grant
  name: Password Grant Flow
  type: oauth2
- evidence: Auth Code OAuth Flow is used for integrations that require using a user’s login to exchange for an access token.
  flows:
  - authorization_code
  name: Auth Code Flow
  type: oauth2
slug: middle-authentication
source_filename: middle-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.middle.app/middle-docs/product/apps/authentication.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.middle.app/middle-docs/product/apps/authentication.md\nsources:\n- https://docs.middle.app/middle-docs/product/apps/authentication.md\n- https://docs.middle.app/middle-docs/product/user-access/multi-factor-authentication.md\n- https://developers.hubspot.com/changelog/new-oauth-v3-api-endpoints-and-standardized-error-responses\n- https://developers.hubspot.com/blog/oauth-token-management-hubspot-integrations\ndescription: Authentication methods supported by Middle as described in the documentation.\nschemes:\n- type: other\n  name: Custom fields\n  evidence: This authentication is best suited for non-OAuth authentications where the system you are integrating with requires an individual\n    username/password, business ID, key, or a predetermined token for each connection.\n- type: oauth2\n  name: Password Grant Flow\n  evidence: The password grant flow is made to support\
  \ the OAuth2.0 Password Grant flow of the same name.\n  flows:\n  - password_grant\n- type: oauth2\n  name: Auth Code Flow\n  evidence: Auth Code OAuth Flow is used for integrations that require using a user’s login to exchange for an access token.\n  flows:\n  - authorization_code\ndocs: https://docs.middle.app/middle-docs/product/apps/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/middle/authentication/middle-authentication.yml
summary_line: 3 schemes
tags:
- Integration Platform
- iPaaS
- Data Integration
---
