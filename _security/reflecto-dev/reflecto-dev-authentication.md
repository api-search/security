---
anonymous_access: false
api_key_in: []
api_specs:
- filename: reflecto-dev-devices-api-openapi.yml
  format: yaml
  label: Reflecto Devices API
  slug: reflecto-dev-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-devices-api-openapi.yml
- filename: reflecto-dev-interactions-api-openapi.yml
  format: yaml
  label: Reflecto Interactions API
  slug: reflecto-dev-interactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-interactions-api-openapi.yml
- filename: reflecto-dev-pushover-compatibility-api-openapi.yml
  format: yaml
  label: Reflecto Pushover compatibility API
  slug: reflecto-dev-pushover-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-pushover-compatibility-api-openapi.yml
- filename: reflecto-dev-reminders-api-openapi.yml
  format: yaml
  label: Reflecto Reminders API
  slug: reflecto-dev-reminders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-reminders-api-openapi.yml
- filename: reflecto-dev-send-api-openapi.yml
  format: yaml
  label: Reflecto Send API
  slug: reflecto-dev-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-send-api-openapi.yml
- filename: reflecto-dev-sms-assistant-api-openapi.yml
  format: yaml
  label: Reflecto SMS (assistant) API
  slug: reflecto-dev-sms-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reflecto-dev/openapi/reflecto-dev-sms-assistant-api-openapi.yml
auth_types: []
description: Reflecto API authenticates every request with an opaque bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Reflecto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reflecto declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Reflecto
provider_slug: reflecto-dev
scheme_count: 1
schemes:
- evidence: The Reflecto API authenticates every request with an opaque bearer token.
  header: Authorization
  how_to_obtain: Tokens are created and managed on your paired Android device; reveal the token in the Android app’s API Tokens screen.
  location: header
  name: Bearer
  type: http-bearer
slug: reflecto-dev-authentication
source_filename: reflecto-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.reflecto.dev/guides/authentication.md
source_yaml: "generated: '2026-11-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.reflecto.dev/guides/authentication.md\nsources:\n- https://docs.reflecto.dev/guides/authentication.md\n- https://docs.reflecto.dev/api-reference/send/send-via-capability-url-path-token-alias.md\n- https://docs.reflecto.dev/guides/quickstart.md\ndescription: Reflecto API authenticates every request with an opaque bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The Reflecto API authenticates every request with an opaque bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Tokens are created and managed on your paired Android device; reveal the token in the Android app’s API Tokens screen.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.reflecto.dev/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/reflecto-dev/authentication/reflecto-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Notification
- Encryption
- Cross-Device
- Open-Source
---
