---
anonymous_access: false
api_key_in: []
api_specs:
- filename: syndigo-openapi-generated.yml
  format: yaml
  label: Syndigo API
  slug: syndigo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndigo/refs/heads/main/openapi/_ae-authored/syndigo-openapi-generated.yml
auth_types: []
description: Syndigo Integration APIs utilize a bearer token authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Syndigo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syndigo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Syndigo
provider_slug: syndigo
scheme_count: 1
schemes:
- evidence: Syndigo Integration APIs utilize a bearer token authentication scheme.
  header: Authorization
  how_to_obtain: Call the Auth API by providing the username and secret as URL parameters or in the request body; extract the "Value" property from the returned JSON object.
  location: header
  name: Bearer Token
  token_url: https://api.uat.syndigo.com/api/auth?username=YourApiUsername&secret=YourUrlEncodedSecret
  type: http-bearer
slug: syndigo-authentication
source_filename: syndigo-authentication.yml
source_heading: Authentication Profile
source_url: https://docx.syndigo.com/developers/docs/api-authentication
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docx.syndigo.com/developers/docs/api-authentication\nsources:\n- https://docx.syndigo.com/developers/docs/api-authentication\n- https://docx.syndigo.com/developers/docs/obtaining-api-keys-and-authenticating-api.md\n- https://docx.syndigo.com/developers/docs/environment-setup.md\n- https://docx.syndigo.com/developers/docs/getting-started-1.md\ndescription: Syndigo Integration APIs utilize a bearer token authentication scheme.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: Syndigo Integration APIs utilize a bearer token authentication scheme.\n  location: header\n  header: Authorization\n  token_url: https://api.uat.syndigo.com/api/auth?username=YourApiUsername&secret=YourUrlEncodedSecret\n  how_to_obtain: Call the Auth API by providing the username and secret as URL parameters or in the request body; extract the \"Value\" property\n    from the returned\
  \ JSON object.\ndocs: https://docx.syndigo.com/developers/docs/api-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syndigo/refs/heads/main/authentication/syndigo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- MasterDataManagement
- ProductInformationManagement
- Syndication
---
