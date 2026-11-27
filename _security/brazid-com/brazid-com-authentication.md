---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brazid-com-openapi-generated.yml
  format: yaml
  label: BrazID API
  slug: brazid-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brazid-com/openapi/_ae-authored/brazid-com-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BrazID Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrazID declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BrazID
provider_slug: brazid-com
scheme_count: 1
schemes:
- evidence: Send your key in the x-api-key header on every request.
  header: x-api-key
  how_to_obtain: Create and revoke keys in the dashboard; a key is generated after confirming your account.
  location: header
  name: API Key
  type: apiKey
slug: brazid-com-authentication
source_filename: brazid-com-authentication.yml
source_heading: Authentication Profile
source_url: https://brazid.com/docs/authentication
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://brazid.com/docs/authentication\nsources:\n- https://brazid.com/docs/authentication\n- https://brazid.com/en/docs/authentication\n- https://brazid.com/es/docs/authentication\n- https://brazid.com/docs/quickstart\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Send your key in the x-api-key header on every request.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create and revoke keys in the dashboard; a key is generated after confirming your account.\ndocs: https://brazid.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/brazid-com/authentication/brazid-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CPF
- CNPJ
- Brazil
- Validation
---
