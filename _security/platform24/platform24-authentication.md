---
anonymous_access: false
api_key_in: []
api_specs:
- filename: platform24-activities-api-openapi.yml
  format: yaml
  label: Platform24 Activities API
  slug: platform24-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-activities-api-openapi.yml
- filename: platform24-data-collect-api-openapi.yml
  format: yaml
  label: Platform24 Data Collect API
  slug: platform24-data-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-data-collect-api-openapi.yml
- filename: platform24-front-door-connect-api-openapi.yml
  format: yaml
  label: Platform24 Front Door Connect API
  slug: platform24-front-door-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-front-door-connect-api-openapi.yml
- filename: platform24-sso-url-api-openapi.yml
  format: yaml
  label: Platform24 Sso Url API
  slug: platform24-sso-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-sso-url-api-openapi.yml
auth_types: []
description: Platform24 uses a custom OAuth 2.0 flow built on the Client Credentials Grant.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Platform24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Platform24 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Platform24
provider_slug: platform24
scheme_count: 1
schemes:
- evidence: '"type":"http","scheme":"basic"'
  flows:
  - client_credentials
  - refresh_token
  - urn:platform24:params:oauth:grant-type:client_credentials_on_behalf_of_patient
  header: Authorization
  how_to_obtain: Provide client_id and client_secret via HTTP Basic Authentication header or as form fields in the token request.
  location: header
  name: BasicAuth
  token_url: https://api.example.com/oauth2/v1/{clientId}/token
  type: http-basic
slug: platform24-authentication
source_filename: platform24-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.platform24.com/front-door-connect/documentation/authentication.md
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.platform24.com/front-door-connect/documentation/authentication.md\nsources:\n- https://docs.platform24.com/front-door-connect/documentation/authentication.md\n- https://docs.platform24.com/front-door-connect/api-reference/authentication.md\n- https://docs.platform24.com/front-door-connect/api-reference/authentication/oauth2.md\n- https://docs.platform24.com/front-door-connect/api-reference/authentication/models.md\ndescription: Platform24 uses a custom OAuth 2.0 flow built on the Client Credentials Grant.\nschemes:\n- type: http-basic\n  name: BasicAuth\n  evidence: '\"type\":\"http\",\"scheme\":\"basic\"'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  - refresh_token\n  - urn:platform24:params:oauth:grant-type:client_credentials_on_behalf_of_patient\n  token_url: https://api.example.com/oauth2/v1/{clientId}/token\n  how_to_obtain:\
  \ Provide client_id and client_secret via HTTP Basic Authentication header or as form fields in the token request.\ndocs: https://docs.platform24.com/front-door-connect/documentation/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/authentication/platform24-authentication.yml
summary_line: 1 scheme
tags:
- Healthcare
- DigitalHealth
- Platform
- PatientEngagement
- Company
---
