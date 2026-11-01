---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zaptec-chargehistory-api-openapi.yml
  format: yaml
  label: Zaptec Charge History API
  slug: zaptec-chargehistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargehistory-api-openapi.yml
- filename: zaptec-charger-api-openapi.yml
  format: yaml
  label: Zaptec Charger API
  slug: zaptec-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-charger-api-openapi.yml
- filename: zaptec-chargerfirmware-api-openapi.yml
  format: yaml
  label: Zaptec Charger Firmware API
  slug: zaptec-chargerfirmware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargerfirmware-api-openapi.yml
- filename: zaptec-constants-api-openapi.yml
  format: yaml
  label: Zaptec Constants API
  slug: zaptec-constants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-constants-api-openapi.yml
- filename: zaptec-installation-api-openapi.yml
  format: yaml
  label: Zaptec Installation API
  slug: zaptec-installation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-installation-api-openapi.yml
- filename: zaptec-session-api-openapi.yml
  format: yaml
  label: Zaptec Session API
  slug: zaptec-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-session-api-openapi.yml
- filename: zaptec-user-group-api-openapi.yml
  format: yaml
  label: Zaptec User Group API
  slug: zaptec-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-user-group-api-openapi.yml
auth_types: []
description: Zaptec uses OAuth 2.0 Resource Owner Password Credentials (ROPC) grant to obtain a bearer token that is sent in the Authorization header. Webhook authentication can also use HTTP Basic when no authentication URL is provided.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zaptec Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zaptec declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zaptec
provider_slug: zaptec
scheme_count: 2
schemes:
- evidence: Authenticate with the ZapCloud API and Zaptec integrations API  by requesting an OAuth bearer token and sending it in the Authorization header for protected API requests.
  flows:
  - password
  header: Authorization
  how_to_obtain: Obtain a user group with owner or service permissions, then POST to https://api.zaptec.com/oauth/token with grant_type=password, username, password, and optional scope=openid.
  location: header
  name: OAuth2 ROPC Bearer Token
  scopes:
  - openid
  token_url: https://api.zaptec.com/oauth/token
  type: http-bearer
- evidence: If an Authentication URL is *not* provided, the username and password from the payload are included in the Authorization header using HTTP Basic authentication.
  header: Authorization
  how_to_obtain: Provide username and password in the webhook payload; Zaptec will include them in the Authorization header using HTTP Basic.
  location: header
  name: Webhook Basic Authentication
  type: http-basic
slug: zaptec-authentication
source_filename: zaptec-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.zaptec.com/docs/api-authentication.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.zaptec.com/docs/api-authentication.md\nsources:\n- https://docs.zaptec.com/docs/api-authentication.md\n- https://docs.zaptec.com/docs/webhook-authentication.md\n- https://docs.zaptec.com/reference/post_chargers-chargerid-onboarding.md\n- https://docs.zaptec.com/reference/post_chargers-chargerid-onboarding\ndescription: Zaptec uses OAuth 2.0 Resource Owner Password Credentials (ROPC) grant to obtain a bearer token that is sent in the Authorization\n  header. Webhook authentication can also use HTTP Basic when no authentication URL is provided.\nschemes:\n- type: http-bearer\n  name: OAuth2 ROPC Bearer Token\n  evidence: Authenticate with the ZapCloud API and Zaptec integrations API  by requesting an OAuth bearer token and sending it in the Authorization\n    header for protected API requests.\n  location: header\n  header: Authorization\n  flows:\n  - password\n  token_url:\
  \ https://api.zaptec.com/oauth/token\n  scopes:\n  - openid\n  how_to_obtain: Obtain a user group with owner or service permissions, then POST to https://api.zaptec.com/oauth/token with grant_type=password,\n    username, password, and optional scope=openid.\n- type: http-basic\n  name: Webhook Basic Authentication\n  evidence: If an Authentication URL is *not* provided, the username and password from the payload are included in the Authorization header using\n    HTTP Basic authentication.\n  location: header\n  header: Authorization\n  how_to_obtain: Provide username and password in the webhook payload; Zaptec will include them in the Authorization header using HTTP Basic.\ndocs: https://docs.zaptec.com/docs/api-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/zaptec/authentication/zaptec-authentication.yml
summary_line: 2 schemes
tags:
- Company
- EVCharging
- SmartCharging
- Energy
- Sustainability
- Platform
---
