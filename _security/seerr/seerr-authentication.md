---
anonymous_access: false
api_key_in: []
api_specs:
- filename: seerr-openapi-generated.yml
  format: yaml
  label: Seerr (Overseerr + Jellyseerr) API
  slug: seerr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seerr/openapi/_ae-authored/seerr-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Seerr API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Seerr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seerr (Overseerr + Jellyseerr) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Seerr (Overseerr + Jellyseerr)
provider_slug: seerr
scheme_count: 1
schemes:
- evidence: Generates a session cookie for use in further requests.
  header: Cookie
  location: header
  name: session cookie
  type: other
slug: seerr-authentication
source_filename: seerr-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.seerr.dev/api/get-main-settings-with-newly-generated-api-key/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.seerr.dev/api/get-main-settings-with-newly-generated-api-key/\nsources:\n- https://docs.seerr.dev/api/get-main-settings-with-newly-generated-api-key/\n- https://docs.seerr.dev/api/sign-in-using-a-plex-token/\n- https://docs.seerr.dev/getting-started/\n- https://docs.seerr.dev/getting-started/buildfromsource/\ndescription: Authentication methods documented for Seerr API.\nschemes:\n- type: other\n  name: session cookie\n  evidence: Generates a session cookie for use in further requests.\n  location: header\n  header: Cookie\ndocs: https://docs.seerr.dev/api/get-main-settings-with-newly-generated-api-key/\n"
source_yaml_url: https://artifacts.apis.io/seerr/authentication/seerr-authentication.yml
summary_line: 1 scheme
tags:
- Media Discovery
- Request Management
- Open Source
- Media Server Integration
- Automation Integration
- Permissions
- Notifications
---
