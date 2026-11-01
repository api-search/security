---
anonymous_access: false
api_key_in: []
api_specs:
- filename: propexo-openapi-generated.yml
  format: yaml
  label: Propexo API
  slug: propexo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propexo/openapi/_ae-authored/propexo-openapi-generated.yml
auth_types: []
description: Propexo API uses a Bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Propexo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Propexo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Propexo
provider_slug: propexo
scheme_count: 1
schemes:
- evidence: When making requests to the Propexo API, you will need to pass proper authentication headers so that you can identify yourself as an authorized user.
  header: Authorization
  how_to_obtain: Contact sales via https://propexo.com/schedule-a-call.
  location: header
  name: Bearer
  type: http-bearer
slug: propexo-authentication
source_filename: propexo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.propexo.com/how-it-works/propexo-api-concepts/authentication.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.propexo.com/how-it-works/propexo-api-concepts/authentication.md\nsources:\n- https://docs.propexo.com/how-it-works/propexo-api-concepts/authentication.md\n- https://docs.propexo.com/pms-guidance/buildium/request-api-key.md\n- https://docs.propexo.com/pms-guidance/rentvine/request-api-key.md\n- https://docs.propexo.com/pms-guidance/yardi/yardi-soap/authentication-errors.md\ndescription: Propexo API uses a Bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: When making requests to the Propexo API, you will need to pass proper authentication headers so that you can identify yourself as\n    an authorized user.\n  location: header\n  header: Authorization\n  how_to_obtain: Contact sales via https://propexo.com/schedule-a-call.\ndocs: https://docs.propexo.com/how-it-works/propexo-api-concepts/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/propexo/authentication/propexo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real Estate
- Data Platform
- Integration
- PropTech
---
