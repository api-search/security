---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mobile-text-alerts-com-openapi-generated.yml
  format: yaml
  label: Mobile Text Alerts API
  slug: mobile-text-alerts-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobile-text-alerts-com/openapi/_ae-authored/mobile-text-alerts-com-openapi-generated.yml
auth_types: []
description: Authentication for Mobile Text Alerts API uses an API Key provided as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mobile Text Alerts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mobile Text Alerts declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mobile Text Alerts
provider_slug: mobile-text-alerts-com
scheme_count: 1
schemes:
- evidence: This **API Key** is used as a bearer token when making requests to the API. A bearer token is included in the request header to grant a user or application access to a protected endpoint.
  header: Authorization
  how_to_obtain: Generate an API Key in the Mobile Text Alerts platform dashboard under Settings → Developer.
  location: header
  name: bearerAuth
  type: http-bearer
slug: mobile-text-alerts-com-authentication
source_filename: mobile-text-alerts-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.mobile-text-alerts.com/getting-started/get-an-api-key.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.mobile-text-alerts.com/getting-started/get-an-api-key.md\nsources:\n- https://developers.mobile-text-alerts.com/getting-started/get-an-api-key.md\n- https://developers.mobile-text-alerts.com/getting-started/send-a-message.md\n- https://developers.mobile-text-alerts.com/getting-started/add-a-subscriber.md\n- https://developers.mobile-text-alerts.com/getting-started/api-basics.md\ndescription: Authentication for Mobile Text Alerts API uses an API Key provided as a Bearer token.\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: This **API Key** is used as a bearer token when making requests to the API. A bearer token is included in the request header to grant\n    a user or application access to a protected endpoint.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API Key in the Mobile Text Alerts platform dashboard under\
  \ Settings → Developer.\nnote: No OAuth2, API key query, or other authentication schemes are documented on the provided pages.\ndocs: https://developers.mobile-text-alerts.com/getting-started/get-an-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/mobile-text-alerts-com/authentication/mobile-text-alerts-com-authentication.yml
summary_line: 1 scheme
tags:
- SMS
- Marketing
- Alerts
- Customer Service
---
