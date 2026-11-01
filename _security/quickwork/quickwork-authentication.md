---
anonymous_access: false
api_key_in: []
api_specs:
- filename: quickwork-embedded-api-openapi.yml
  format: yaml
  label: Quickwork Embedded API
  slug: quickwork-embedded-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickwork/openapi/quickwork-embedded-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the page
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Quickwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quickwork declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Quickwork
provider_slug: quickwork
scheme_count: 1
schemes:
- evidence: 'Enter in format: api-key <partner_token>'
  header: Authorization
  location: header
  name: Authorization
  type: apiKey
slug: quickwork-authentication
source_filename: quickwork-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.quickwork.co/reference/create_user_token.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.quickwork.co/reference/create_user_token.md\nsources:\n- https://docs.quickwork.co/reference/create_user_token.md\ndescription: Authentication schemes as published on the page\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Enter in format: api-key <partner_token>'\n  location: header\n  header: Authorization\nnote: Only the apiKey scheme is defined; no OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://docs.quickwork.co/reference/create_user_token.md\n"
source_yaml_url: https://artifacts.apis.io/quickwork/authentication/quickwork-authentication.yml
summary_line: 1 scheme
tags:
- Integration
- Automation
- Workflows
- API Platform
- Enterprise
---
