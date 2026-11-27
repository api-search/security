---
anonymous_access: false
api_key_in: []
api_specs:
- filename: labii-openapi-generated.yml
  format: yaml
  label: Labii API
  slug: labii-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/labii/openapi/_ae-authored/labii-openapi-generated.yml
auth_types: []
description: Authentication schemes extracted from Labii documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Labii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Labii declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Labii
provider_slug: labii
scheme_count: 1
schemes:
- evidence: 'Parameter: `token` (header, string)'
  header: token
  location: header
  name: token
  type: other
slug: labii-authentication
source_filename: labii-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.labii.com/user-guide/start-here/accounts/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.labii.com/user-guide/start-here/accounts/authentication.md\nsources:\n- https://docs.labii.com/user-guide/start-here/accounts/authentication.md\n- https://docs.labii.com/admin-guide/api-keys.md\n- https://docs.labii.com/api/methods/authentication.md\n- https://docs.labii.com/api/concepts/how-to-get-token-from-labii-eln-and-lims.md\ndescription: Authentication schemes extracted from Labii documentation.\nschemes:\n- type: other\n  name: token\n  evidence: 'Parameter: `token` (header, string)'\n  location: header\n  header: token\ndocs: https://docs.labii.com/user-guide/start-here/accounts/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/labii/authentication/labii-authentication.yml
summary_line: 1 scheme
tags:
- Company
- ELN
- LIMS
- Laboratory
- Digital Health
- Software-as-a-Service
---
