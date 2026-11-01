---
anonymous_access: false
api_key_in: []
api_specs:
- filename: saga-it-openapi-generated.yml
  format: yaml
  label: Saga IT API
  slug: saga-it-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/saga-it/openapi/_ae-authored/saga-it-openapi-generated.yml
auth_types: []
description: Authentication for MirthSync is performed using HTTP Basic authentication with a username and password. Credentials can be supplied via command‑line options (-u and -p) or through the MIRTHSYNC_PASSWORD environment variable.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Saga It Authentication
name_suffix: Authentication
oauth_flows: []
overview: Saga IT declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Saga IT
provider_slug: saga-it
scheme_count: 1
schemes:
- evidence: Server credentials can be provided via command-line options or environment variables for security.
  header: Authorization
  how_to_obtain: Provide username with -u and password with -p flags, or set MIRTHSYNC_PASSWORD environment variable.
  location: header
  name: Mirth Connect API
  type: http-basic
slug: saga-it-authentication
source_filename: saga-it-authentication.yml
source_heading: Authentication Profile
source_url: https://saga-it.com/docs/mirthsync/cli/setup
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://saga-it.com/docs/mirthsync/cli/setup\nsources:\n- https://saga-it.com/docs/mirthsync/cli/setup\n- https://saga-it.com/docs/mirthsync/ide/setup\n- https://saga-it.com/docs/mirthsync/guides/ci-cd-setup\ndescription: Authentication for MirthSync is performed using HTTP Basic authentication with a username and password. Credentials can be supplied\n  via command‑line options (-u and -p) or through the MIRTHSYNC_PASSWORD environment variable.\nschemes:\n- type: http-basic\n  name: Mirth Connect API\n  evidence: Server credentials can be provided via command-line options or environment variables for security.\n  location: header\n  header: Authorization\n  how_to_obtain: Provide username with -u and password with -p flags, or set MIRTHSYNC_PASSWORD environment variable.\ndocs: https://saga-it.com/docs/mirthsync/cli/setup\n"
source_yaml_url: https://artifacts.apis.io/saga-it/authentication/saga-it-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- IT Consulting
- Interoperability
- Cloud Services
---
