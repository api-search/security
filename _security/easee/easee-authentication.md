---
anonymous_access: false
api_key_in: []
api_specs:
- filename: easee-account-api-openapi.yml
  format: yaml
  label: Easee Account API
  slug: easee-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-account-api-openapi.yml
- filename: easee-authorizecharging-api-openapi.yml
  format: yaml
  label: Easee Authorize Charging API
  slug: easee-authorizecharging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-authorizecharging-api-openapi.yml
- filename: easee-charge-session-api-openapi.yml
  format: yaml
  label: Easee Charge Session API
  slug: easee-charge-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-charge-session-api-openapi.yml
- filename: easee-charger-api-openapi.yml
  format: yaml
  label: Easee Charger API
  slug: easee-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-charger-api-openapi.yml
- filename: easee-cloud-ocpp-api-openapi.yml
  format: yaml
  label: Easee Cloud OCPP API
  slug: easee-cloud-ocpp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-cloud-ocpp-api-openapi.yml
- filename: easee-daily-schedule-api-openapi.yml
  format: yaml
  label: Easee Daily schedule API
  slug: easee-daily-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-daily-schedule-api-openapi.yml
- filename: easee-delayed-schedule-api-openapi.yml
  format: yaml
  label: Easee Delayed schedule API
  slug: easee-delayed-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-delayed-schedule-api-openapi.yml
- filename: easee-direct-ocpp-for-operators-api-openapi.yml
  format: yaml
  label: Easee Direct OCPP - For Operators API
  slug: easee-direct-ocpp-for-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-direct-ocpp-for-operators-api-openapi.yml
- filename: easee-direct-ocpp-for-users-api-openapi.yml
  format: yaml
  label: Easee Direct OCPP - For Users API
  slug: easee-direct-ocpp-for-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-direct-ocpp-for-users-api-openapi.yml
- filename: easee-easeekeys-api-openapi.yml
  format: yaml
  label: Easee Easee Keys API
  slug: easee-easeekeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-easeekeys-api-openapi.yml
- filename: easee-energy-reporting-api-openapi.yml
  format: yaml
  label: Easee Energy Reporting API
  slug: easee-energy-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-energy-reporting-api-openapi.yml
- filename: easee-equalizer-api-openapi.yml
  format: yaml
  label: Easee Equalizer API
  slug: easee-equalizer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-equalizer-api-openapi.yml
- filename: easee-observations-api-openapi.yml
  format: yaml
  label: Easee Observations API
  slug: easee-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-observations-api-openapi.yml
- filename: easee-resources-api-openapi.yml
  format: yaml
  label: Easee Resources API
  slug: easee-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-resources-api-openapi.yml
- filename: easee-site-api-openapi.yml
  format: yaml
  label: Easee Site API
  slug: easee-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-site-api-openapi.yml
- filename: easee-site-charge-session-api-openapi.yml
  format: yaml
  label: Easee Site Charge Session API
  slug: easee-site-charge-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-site-charge-session-api-openapi.yml
- filename: easee-state-api-openapi.yml
  format: yaml
  label: Easee State API
  slug: easee-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-state-api-openapi.yml
- filename: easee-weekly-schedule-api-openapi.yml
  format: yaml
  label: Easee Weekly schedule API
  slug: easee-weekly-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-weekly-schedule-api-openapi.yml
auth_types: []
description: Authentication methods for Easee APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Easee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Easee declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Easee
provider_slug: easee
scheme_count: 2
schemes:
- evidence: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  header: Authorization
  how_to_obtain: Call the /api/accounts/login endpoint with a JSON body containing userName and password to receive an accessToken and refreshToken.
  location: header
  name: Bearer
  type: apiKey
- authorize_url: https://auth.easee.com/realms/easee/protocol/openid-connect/auth
  evidence: Easee supports OAuth 2.0 based on the OAuth 2.0 Authorization Framework (RFC 6749) and follows the standard authorization code flow for user-delegated access.
  how_to_obtain: Register an application to receive a client_id (and client_secret if confidential), then perform the Authorization Code flow with PKCE as described in the OAuth 2.0 Integration Guide.
  name: OAuth2 Authorization Code with PKCE
  scopes:
  - openid
  - profile
  - email
  - chargers:read
  - sites:read
  - sites:operator:manage
  - sessions:read
  - account:profile:read
  - equalizers:read
  token_url: https://auth.easee.com/realms/easee/protocol/openid-connect/token
  type: oauth2
slug: easee-authentication
source_filename: easee-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.easee.com/docs/authentication-1.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.easee.com/docs/authentication-1.md\nsources:\n- https://developer.easee.com/docs/authentication-1.md\n- https://developer.easee.com/docs/oauth-20-integration-guide.md\n- https://developer.easee.com/docs/available-oauth-scopes.md\n- https://developer.easee.com/reference/account_authenticate.md\ndescription: Authentication methods for Easee APIs\nschemes:\n- type: apiKey\n  name: Bearer\n  evidence: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer {token}\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Call the /api/accounts/login endpoint with a JSON body containing userName and password to receive an accessToken and refreshToken.\n- type: oauth2\n  name: OAuth2 Authorization Code with PKCE\n  evidence: Easee supports OAuth 2.0 based on the OAuth 2.0 Authorization Framework (RFC 6749) and follows the standard\
  \ authorization code flow\n    for user-delegated access.\n  token_url: https://auth.easee.com/realms/easee/protocol/openid-connect/token\n  authorize_url: https://auth.easee.com/realms/easee/protocol/openid-connect/auth\n  scopes:\n  - openid\n  - profile\n  - email\n  - chargers:read\n  - sites:read\n  - sites:operator:manage\n  - sessions:read\n  - account:profile:read\n  - equalizers:read\n  how_to_obtain: Register an application to receive a client_id (and client_secret if confidential), then perform the Authorization Code flow\n    with PKCE as described in the OAuth 2.0 Integration Guide.\ndocs: https://developer.easee.com/docs/authentication-1.md\n"
source_yaml_url: https://artifacts.apis.io/easee/authentication/easee-authentication.yml
summary_line: 2 schemes
tags:
- Company
- EVCharging
- SmartHome
- IoT
- Energy
---
