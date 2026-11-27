---
anonymous_access: false
api_key_in: []
api_specs:
- filename: numezis-com-openapi-generated.yml
  format: yaml
  label: Numezis API
  slug: numezis-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numezis-com/openapi/_ae-authored/numezis-com-openapi-generated.yml
auth_types: []
description: Authentication schemes published for Numezis API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Numezis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numezis declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Numezis
provider_slug: numezis-com
scheme_count: 1
schemes:
- evidence: The web app uses HttpOnly session cookies after POST /auth/login .
  how_to_obtain: Obtain a session cookie by POSTing credentials to /auth/login.
  location: cookie
  name: session cookie
  type: other
slug: numezis-com-authentication
source_filename: numezis-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.numezis.com/en/docs/developer/authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.numezis.com/en/docs/developer/authentication\nsources:\n- https://docs.numezis.com/en/docs/developer/authentication\n- https://docs.numezis.com/en/docs/getting-started/for-developers\n- https://docs.numezis.com/en/docs/getting-started/connect-bank\ndescription: Authentication schemes published for Numezis API\nschemes:\n- type: other\n  name: session cookie\n  evidence: The web app uses HttpOnly session cookies after POST /auth/login .\n  location: cookie\n  how_to_obtain: Obtain a session cookie by POSTing credentials to /auth/login.\ndocs: https://docs.numezis.com/en/docs/developer/authentication\n"
source_yaml_url: https://artifacts.apis.io/numezis-com/authentication/numezis-com-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- AI Agents
- Swiss SMEs
- ERP Integration
- Payroll
- VAT
- Invoicing
---
