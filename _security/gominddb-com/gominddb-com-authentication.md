---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gominddb-com-openapi-generated.yml
  format: yaml
  label: Gomind API
  slug: gominddb-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gominddb-com/openapi/_ae-authored/gominddb-com-openapi-generated.yml
auth_types: []
description: Gomind uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gomind Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gomind declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gomind
provider_slug: gominddb-com
scheme_count: 1
schemes:
- evidence: 'curl https://api.gominddb.com/v1/remember \ -H "Authorization: Bearer $GOMIND_API_KEY" \'
  header: Authorization
  how_to_obtain: Create an organization and an API key in the Gomind dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: gominddb-com-authentication
source_filename: gominddb-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gominddb.ai/en/docs/quickstart
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gominddb.ai/en/docs/quickstart\nsources:\n- https://gominddb.ai/en/docs/quickstart\ndescription: Gomind uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl https://api.gominddb.com/v1/remember \\ -H \"Authorization: Bearer $GOMIND_API_KEY\" \\'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an organization and an API key in the Gomind dashboard.\ndocs: https://gominddb.ai/en/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/gominddb-com/authentication/gominddb-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Collaboration
- Knowledge Management
- Teamwork
---
