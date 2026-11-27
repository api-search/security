---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published on CiteHawk documentation
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CiteHawk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CiteHawk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CiteHawk
provider_slug: citehawk-com
scheme_count: 1
schemes:
- evidence: 'Pass the key as a Bearer token on every request: Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create a key in the workspace Settings > API Keys card, give it a name, choose scopes and expiry, and copy the shown key.
  location: header
  name: API Key
  scopes:
  - read:brands
  - read:metrics
  - read:responses
  - read:scores
  - write:prospect-scans
  type: http-bearer
slug: citehawk-com-authentication
source_filename: citehawk-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.citehawk.com/docs/api-keys
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.citehawk.com/docs/api-keys\nsources:\n- https://www.citehawk.com/docs/api-keys\n- https://dev.citehawk.com/leaderboards/auth-platforms\n- https://www.citehawk.com/leaderboards/auth-platforms\n- https://www.citehawk.com/learn/guides/getting-started\ndescription: Authentication methods published on CiteHawk documentation\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Pass the key as a Bearer token on every request: Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  scopes:\n  - read:brands\n  - read:metrics\n  - read:responses\n  - read:scores\n  - write:prospect-scans\n  how_to_obtain: Create a key in the workspace Settings > API Keys card, give it a name, choose scopes and expiry, and copy the shown key.\nnote: No OAuth2, API key, or other authentication schemes were found on the provided pages.\ndocs: https://www.citehawk.com/docs/api-keys\n"
source_yaml_url: https://artifacts.apis.io/citehawk-com/authentication/citehawk-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Visibility
- Brands
- Monitoring
---
