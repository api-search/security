---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for ORYKSA API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ORYKSA Authentication
name_suffix: Authentication
oauth_flows: []
overview: ORYKSA declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ORYKSA
provider_slug: oryksa-com
scheme_count: 2
schemes:
- evidence: Send the key in the Authorization header as a bearer token (the X-API-Key header also works).
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: Send the key in the Authorization header as a bearer token (the X-API-Key header also works).
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: oryksa-com-authentication
source_filename: oryksa-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.oryksa.com/en/a/two-factor-authentication
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.oryksa.com/en/a/two-factor-authentication\nsources:\n- https://help.oryksa.com/en/a/two-factor-authentication\n- https://developer.oryksa.com/en/authentication\n- https://developer.oryksa.com/pt/authentication\n- https://developer.oryksa.com/br/authentication\ndescription: Authentication schemes for ORYKSA API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Send the key in the Authorization header as a bearer token (the X-API-Key header also works).\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-API-Key\n  evidence: Send the key in the Authorization header as a bearer token (the X-API-Key header also works).\n  location: header\n  header: X-API-Key\nnote: No OAuth2 flows or other authentication methods are documented on the provided pages.\ndocs: https://help.oryksa.com/en/a/two-factor-authentication\n"
source_yaml_url: https://artifacts.apis.io/oryksa-com/authentication/oryksa-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Automation
- Sales
- Customer Service
- Software-as-a-Service
---
