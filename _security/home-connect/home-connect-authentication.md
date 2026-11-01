---
anonymous_access: false
api_key_in: []
api_specs:
- filename: home-connect-appliances-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Appliances API
  slug: home-connect-appliances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-appliances-api-openapi.yml
- filename: home-connect-commands-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Commands API
  slug: home-connect-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-commands-api-openapi.yml
- filename: home-connect-events-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Events API
  slug: home-connect-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-events-api-openapi.yml
- filename: home-connect-images-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Images API
  slug: home-connect-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-images-api-openapi.yml
- filename: home-connect-map-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Map API
  slug: home-connect-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-map-api-openapi.yml
- filename: home-connect-programs-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Programs API
  slug: home-connect-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-programs-api-openapi.yml
- filename: home-connect-settings-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Settings API
  slug: home-connect-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-settings-api-openapi.yml
- filename: home-connect-status-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Status API
  slug: home-connect-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-status-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Home Connect Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Home Connect (BSH appliances) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Home Connect (BSH appliances)
provider_slug: home-connect
scheme_count: 1
schemes:
- description: 'The Home Connect API uses the authorization code grant flow of the OAuth2

    Authorization Framework as specified in RFC 6749 (https://tools.ietf.org/html/rfc6749).

    Authorization tokens have to be transmitted in the HTTP headers as defined

    in RFC 6750 (https://tools.ietf.org/html/rfc6750).'
  flows:
  - authorizationUrl: https://api.home-connect.com/security/oauth/authorize
    flow: authorizationCode
    scopes: 63
    tokenUrl: https://api.home-connect.com/security/oauth/token
  name: homeconnect_auth
  sources:
  - openapi/home-connect-openapi.yaml
  type: oauth2
slug: home-connect-authentication
source_filename: home-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/home-connect-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: homeconnect_auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.home-connect.com/security/oauth/authorize\n    tokenUrl: https://api.home-connect.com/security/oauth/token\n    scopes: 63\n  description: |-\n    The Home Connect API uses the authorization code grant flow of the OAuth2\n    Authorization Framework as specified in RFC 6749 (https://tools.ietf.org/html/rfc6749).\n    Authorization tokens have to be transmitted in the HTTP headers as defined\n    in RFC 6750 (https://tools.ietf.org/html/rfc6750).\n  sources:\n  - openapi/home-connect-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/home-connect/authentication/home-connect-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- smart home
- appliances
- connected devices
---
