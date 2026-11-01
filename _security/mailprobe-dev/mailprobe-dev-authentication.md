---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailprobe-dev-account-api-openapi.yml
  format: yaml
  label: mailprobe-dev Account API
  slug: mailprobe-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailprobe-dev/openapi/mailprobe-dev-account-api-openapi.yml
- filename: mailprobe-dev-verification-api-openapi.yml
  format: yaml
  label: mailprobe-dev Verification API
  slug: mailprobe-dev-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailprobe-dev/openapi/mailprobe-dev-verification-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailprobe Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: mailprobe-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mailprobe-dev
provider_slug: mailprobe-dev
scheme_count: 1
schemes:
- evidence: All API requests require authentication via your API key in the Authorization header.
  header: Authorization
  how_to_obtain: Create a key under Developer in your account; the key is shown once at creation.
  location: header
  name: API Key
  type: http-bearer
slug: mailprobe-dev-authentication
source_filename: mailprobe-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://mailprobe.dev/blog/spf-dkim-dmarc-email-authentication-explained/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailprobe.dev/blog/spf-dkim-dmarc-email-authentication-explained/\nsources:\n- https://mailprobe.dev/blog/spf-dkim-dmarc-email-authentication-explained/\n- https://mailprobe.dev/api-docs/#mcp\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: All API requests require authentication via your API key in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key under Developer in your account; the key is shown once at creation.\ndocs: https://mailprobe.dev/blog/spf-dkim-dmarc-email-authentication-explained/\n"
source_yaml_url: https://artifacts.apis.io/mailprobe-dev/authentication/mailprobe-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email Verification
- API
- Real-time
- Developer Tools
---
