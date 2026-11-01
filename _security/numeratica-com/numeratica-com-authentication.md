---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Numeratica API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Numeratica Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: numeratica-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: numeratica-com
provider_slug: numeratica-com
scheme_count: 1
schemes:
- evidence: Every /v1 call takes an API key as a bearer token.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: numeratica-com-authentication
source_filename: numeratica-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.numeratica.com/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.numeratica.com/\nsources:\n- https://docs.numeratica.com/\ndescription: Authentication schemes for Numeratica API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every /v1 call takes an API key as a bearer token.\n  location: header\n  header: Authorization\ndocs: https://docs.numeratica.com/\n"
source_yaml_url: https://artifacts.apis.io/numeratica-com/authentication/numeratica-com-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- API
- Calculators
- Retirement
- Household
---
