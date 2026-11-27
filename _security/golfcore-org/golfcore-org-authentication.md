---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for GolfCore Course Data API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GolfCore Authentication
name_suffix: Authentication
oauth_flows: []
overview: GolfCore declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GolfCore
provider_slug: golfcore-org
scheme_count: 1
schemes:
- evidence: 'Send it curl "https://api.golfcore.org/v1/courses/pebble-beach" \ -H "Authorization: Bearer gc_live_..."'
  header: Authorization
  how_to_obtain: Sign in at platform.golfcore.app with your GolfCore account, accept the API terms and create a key. The secret is shown once.
  location: header
  name: Bearer
  type: http-bearer
slug: golfcore-org-authentication
source_filename: golfcore-org-authentication.yml
source_heading: Authentication Profile
source_url: https://www.golfcore.org/developers/
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.golfcore.org/developers/\nsources:\n- https://www.golfcore.org/developers/\n- https://www.golfcore.org/developers/keys/\ndescription: Authentication for GolfCore Course Data API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it curl \"https://api.golfcore.org/v1/courses/pebble-beach\" \\ -H \"Authorization: Bearer gc_live_...\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in at platform.golfcore.app with your GolfCore account, accept the API terms and create a key. The secret is shown once.\ndocs: https://www.golfcore.org/developers/\n"
source_yaml_url: https://artifacts.apis.io/golfcore-org/authentication/golfcore-org-authentication.yml
summary_line: 1 scheme
tags:
- Golf
- GPS
- Sports
- Mobile App
---
