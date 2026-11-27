---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Carousel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carousel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Carousel
provider_slug: oncarousel-com
scheme_count: 1
schemes:
- evidence: 'Every request carries Authorization: Bearer <your key>.'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: oncarousel-com-authentication
source_filename: oncarousel-com-authentication.yml
source_heading: Authentication Profile
source_url: https://oncarousel.com/docs/tokens/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://oncarousel.com/docs/tokens/\nsources:\n- https://oncarousel.com/docs/tokens/\n- https://oncarousel.com/docs/tokens/\n- https://oncarousel.com/docs/\n- https://oncarousel.com/docs/api-quickstart/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request carries Authorization: Bearer <your key>.'\n  location: header\n  header: Authorization\ndocs: https://oncarousel.com/docs/tokens/\n"
source_yaml_url: https://artifacts.apis.io/oncarousel-com/authentication/oncarousel-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Lending
- Tenant Screening
- API Platform
---
