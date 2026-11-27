---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for MetaRun's App Store Connect API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MetaRun Authentication
name_suffix: Authentication
oauth_flows: []
overview: MetaRun declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MetaRun
provider_slug: metarun-dev
scheme_count: 1
schemes:
- evidence: 'It goes in an Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: 'Sign a JWT with the .p8 private key (ES256) using the Key ID (kid) and Issuer ID (iss); the resulting token is placed in the Authorization: Bearer header.'
  location: header
  name: App Store Connect API token
  type: http-bearer
slug: metarun-dev-authentication
source_filename: metarun-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://metarun.dev/guides/app-store-connect-api-key
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://metarun.dev/guides/app-store-connect-api-key\nsources:\n- https://metarun.dev/guides/app-store-connect-api-key\n- https://metarun.dev/guides/testflight-external-testers\ndescription: Authentication for MetaRun's App Store Connect API\nschemes:\n- type: http-bearer\n  name: App Store Connect API token\n  evidence: 'It goes in an Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Sign a JWT with the .p8 private key (ES256) using the Key ID (kid) and Issuer ID (iss); the resulting token is placed in the\n    Authorization: Bearer header.'\ndocs: https://metarun.dev/guides/app-store-connect-api-key\n"
source_yaml_url: https://artifacts.apis.io/metarun-dev/authentication/metarun-dev-authentication.yml
summary_line: 1 scheme
tags:
- App Store Connect
- AI Agents
- Pricing
- Localization
---
