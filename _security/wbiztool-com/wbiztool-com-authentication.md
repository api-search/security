---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wbiztool-com-account-api-openapi.yml
  format: yaml
  label: wbiztool-com Account API
  slug: wbiztool-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-account-api-openapi.yml
- filename: wbiztool-com-media-api-openapi.yml
  format: yaml
  label: wbiztool-com Media API
  slug: wbiztool-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-media-api-openapi.yml
- filename: wbiztool-com-messages-api-openapi.yml
  format: yaml
  label: wbiztool-com Messages API
  slug: wbiztool-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-messages-api-openapi.yml
- filename: wbiztool-com-number-verification-api-openapi.yml
  format: yaml
  label: wbiztool-com Number verification API
  slug: wbiztool-com-number-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-number-verification-api-openapi.yml
- filename: wbiztool-com-reminders-api-openapi.yml
  format: yaml
  label: wbiztool-com Reminders API
  slug: wbiztool-com-reminders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-reminders-api-openapi.yml
- filename: wbiztool-com-whatsapp-numbers-api-openapi.yml
  format: yaml
  label: wbiztool-com WhatsApp numbers API
  slug: wbiztool-com-whatsapp-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-whatsapp-numbers-api-openapi.yml
auth_types: []
description: 'Authentication uses an API key sent in an Authorization: Bearer header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wbiztool Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: wbiztool-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: wbiztool-com
provider_slug: wbiztool-com
scheme_count: 1
schemes:
- evidence: 'Your own code sends the key in an Authorization: Bearer header; integrations ask for two values from the API keys page: your workspace''s Client ID and one of its keys.'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API keys; the key is displayed once and can be copied.
  location: header
  name: Bearer
  type: http-bearer
slug: wbiztool-com-authentication
source_filename: wbiztool-com-authentication.yml
source_heading: Authentication Profile
source_url: https://wbiztool.com/docs/guides/api-keys/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://wbiztool.com/docs/guides/api-keys/\nsources:\n- https://wbiztool.com/docs/guides/api-keys/\n- https://wbiztool.com/docs/guides/api-keys/\n- https://wbiztool.com/docs/check-my-creds-api/\n- https://wbiztool.com/docs/check-my-creds-api/\ndescription: 'Authentication uses an API key sent in an Authorization: Bearer header.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Your own code sends the key in an Authorization: Bearer header; integrations ask for two values from the API keys page: your workspace''s\n    Client ID and one of its keys.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API keys; the key is displayed once and can be copied.\ndocs: https://wbiztool.com/docs/guides/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/wbiztool-com/authentication/wbiztool-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- WhatsApp
- Messaging
- Automation
- Business
---
