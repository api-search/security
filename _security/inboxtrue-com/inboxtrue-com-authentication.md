---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inboxtrue-com-email-api-openapi.yml
  format: yaml
  label: InboxTrue Email API
  slug: inboxtrue-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxtrue-com/openapi/inboxtrue-com-email-api-openapi.yml
- filename: inboxtrue-com-zeroclick-api-openapi.yml
  format: yaml
  label: InboxTrue Zeroclick API
  slug: inboxtrue-com-zeroclick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxtrue-com/openapi/inboxtrue-com-zeroclick-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: InboxTrue Authentication
name_suffix: Authentication
oauth_flows: []
overview: InboxTrue declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: InboxTrue
provider_slug: inboxtrue-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Sign up to create an account and receive an API key.
  location: header
  name: Bearer
  type: http-bearer
slug: inboxtrue-com-authentication
source_filename: inboxtrue-com-authentication.yml
source_heading: Authentication Profile
source_url: https://inboxtrue.com/register
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://inboxtrue.com/register\nsources:\n- https://inboxtrue.com/register\n- https://inboxtrue.com/#developers\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up to create an account and receive an API key.\ndocs: https://inboxtrue.com/register\n"
source_yaml_url: https://artifacts.apis.io/inboxtrue-com/authentication/inboxtrue-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email Verification
- Software-as-a-Service
- Developer Tools
---
