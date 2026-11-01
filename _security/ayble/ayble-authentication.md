---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ayble-openapi-generated.yml
  format: yaml
  label: Ayble API
  slug: ayble-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayble/openapi/_ae-authored/ayble-openapi-generated.yml
auth_types: []
description: Authentication schemes for Ashby API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ayble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ayble declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ayble
provider_slug: ayble
scheme_count: 1
schemes:
- evidence: Use HTTP Basic Auth to authenticate with our API.
  header: Authorization
  how_to_obtain: Generate an API key in Admin > Integrations > API Credentials and use it as the basic auth username; leave the password blank.
  location: header
  name: Basic
  type: http-basic
slug: ayble-authentication
source_filename: ayble-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.ashbyhq.com/reference/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.ashbyhq.com/reference/authentication.md\nsources:\n- https://developers.ashbyhq.com/reference/authentication.md\n- https://docs.ashbyhq.com/how-do-i-generate-an-api-key\n- https://docs.ashbyhq.com/google-workspace-individual-oauth\n- https://docs.ashbyhq.com/there-was-an-authentication-error-please-check-your-credentials-and-their-permissions-are-correct-what-should-i-do\ndescription: Authentication schemes for Ashby API\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: Use HTTP Basic Auth to authenticate with our API.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in Admin > Integrations > API Credentials and use it as the basic auth username; leave the password blank.\ndocs: https://developers.ashbyhq.com/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/ayble/authentication/ayble-authentication.yml
summary_line: 1 scheme
tags:
- Health
- Telemedicine
- DigestiveHealth
- VirtualClinic
- EmployerBenefits
- Healthcare
---
