---
anonymous_access: false
api_key_in: []
auth_types: []
description: API key authentication using a Bearer token
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: A2A Infrastructure Authentication
name_suffix: Authentication
oauth_flows: []
overview: A2A Infrastructure declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: A2A Infrastructure
provider_slug: a2ainfrastructure-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer a2a_YOUR_KEY'
  header: Authorization
  how_to_obtain: Create an API key in the dashboard; the key starts with a2a_ and is returned by the signup endpoint.
  location: header
  name: Bearer token
  type: http-bearer
slug: a2ainfrastructure-com-authentication
source_filename: a2ainfrastructure-com-authentication.yml
source_heading: Authentication Profile
source_url: https://a2ainfrastructure.com/auth/signup
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://a2ainfrastructure.com/auth/signup\nsources:\n- https://a2ainfrastructure.com/auth/signup\n- https://a2ainfrastructure.com/auth/login\n- https://a2ainfrastructure.com/quickstart\n- https://a2ainfrastructure.com/quickstart/rest\ndescription: API key authentication using a Bearer token\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authorization: Bearer a2a_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard; the key starts with a2a_ and is returned by the signup endpoint.\ndocs: https://a2ainfrastructure.com/auth/signup\n"
source_yaml_url: https://artifacts.apis.io/a2ainfrastructure-com/authentication/a2ainfrastructure-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Compliance
- Enterprise
- Governance
- Infrastructure
---
