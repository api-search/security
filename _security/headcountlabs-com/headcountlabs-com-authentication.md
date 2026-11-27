---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Headcount Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Headcount Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Headcount Labs
provider_slug: headcountlabs-com
scheme_count: 1
schemes:
- evidence: 'Every request to the API carries your key in the Authorization header: Authorization: Bearer <API_KEY>'
  header: Authorization
  how_to_obtain: Sign in at https://api.headcountlabs.com/data/login and create keys at https://api.headcountlabs.com/data/keys
  location: header
  name: Bearer API key
  type: http-bearer
slug: headcountlabs-com-authentication
source_filename: headcountlabs-com-authentication.yml
source_heading: Authentication Profile
source_url: https://headcountlabs.com/docs/authentication/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://headcountlabs.com/docs/authentication/\nsources:\n- https://headcountlabs.com/docs/authentication/\n- https://headcountlabs.com/docs/authentication.md\n- https://headcountlabs.com/docs/authentication/\n- https://headcountlabs.com/docs/getting-started/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer API key\n  evidence: 'Every request to the API carries your key in the Authorization header: Authorization: Bearer <API_KEY>'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in at https://api.headcountlabs.com/data/login and create keys at https://api.headcountlabs.com/data/keys\nnote: No OAuth flows are described for this API.\ndocs: https://headcountlabs.com/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/headcountlabs-com/authentication/headcountlabs-com-authentication.yml
summary_line: 1 scheme
tags:
- Job
- Data
- Recruiting
- Employment
---
