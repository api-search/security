---
anonymous_access: false
api_key_in: []
api_specs:
- filename: securessmtp-com-openapi-generated.yml
  format: yaml
  label: securessmtp-com API
  slug: securessmtp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/securessmtp-com/openapi/_ae-authored/securessmtp-com-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on SecureSMTP documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Securessmtp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: securessmtp-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: securessmtp-com
provider_slug: securessmtp-com
scheme_count: 1
schemes:
- evidence: 'The same key works everywhere: in the x-securessmtp-api-key header for the API, in the WordPress plugin, as the SMTP password, and as a bearer token for the MCP server.'
  header: x-securessmtp-api-key
  how_to_obtain: The API key is shown in full once when the site is created and emailed to the account owner.
  location: header
  name: x-securessmtp-api-key
  type: apiKey
slug: securessmtp-com-authentication
source_filename: securessmtp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://securessmtp.com/docs/guides/sites-and-keys
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://securessmtp.com/docs/guides/sites-and-keys\nsources:\n- https://securessmtp.com/docs/guides/sites-and-keys\n- https://securessmtp.com/docs/guides/quickstart\ndescription: Authentication schemes as published on SecureSMTP documentation.\nschemes:\n- type: apiKey\n  name: x-securessmtp-api-key\n  evidence: 'The same key works everywhere: in the x-securessmtp-api-key header for the API, in the WordPress plugin, as the SMTP password, and\n    as a bearer token for the MCP server.'\n  location: header\n  header: x-securessmtp-api-key\n  how_to_obtain: The API key is shown in full once when the site is created and emailed to the account owner.\ndocs: https://securessmtp.com/docs/guides/sites-and-keys\n"
source_yaml_url: https://artifacts.apis.io/securessmtp-com/authentication/securessmtp-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Transactional
- API
- SMTP
- Service
- SecureSMTP
---
