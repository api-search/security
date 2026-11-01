---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eagle-doc-doc-api-openapi.yml
  format: yaml
  label: Eagle Doc API
  slug: eagle-doc-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eagle-doc/openapi/eagle-doc-doc-api-openapi.yml
- filename: eagle-doc-openapi-generated.yml
  format: yaml
  label: Eagle Doc API
  slug: eagle-doc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eagle-doc/openapi/_ae-authored/eagle-doc-openapi-generated.yml
auth_types: []
description: A business API key authenticates machine calls as your business rather than as a person. You send it in the same api-key header you already use for personal keys — the only difference is the APIB- prefix.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Eagle Doc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eagle Doc declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Eagle Doc
provider_slug: eagle-doc
scheme_count: 1
schemes:
- evidence: A business API key authenticates machine calls as your business rather than as a person. You send it in the same api-key header you already use for personal keys — the only difference is the APIB- prefix.
  header: api-key
  how_to_obtain: Create, rename and revoke business API keys through the management API or from the dashboard. Rotate a key by creating a new one and revoking the old one.
  location: header
  name: api-key
  type: apiKey
slug: eagle-doc-authentication
source_filename: eagle-doc-authentication.yml
source_heading: Authentication Profile
source_url: https://www.eagle-doc.com/en/documentation/business-api/authentication/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.eagle-doc.com/en/documentation/business-api/authentication/\nsources:\n- https://www.eagle-doc.com/en/documentation/business-api/authentication/\n- https://www.eagle-doc.com/de/documentation/business-api/authentication/\ndescription: A business API key authenticates machine calls as your business rather than as a person. You send it in the same api-key header you\n  already use for personal keys — the only difference is the APIB- prefix.\nschemes:\n- type: apiKey\n  name: api-key\n  evidence: A business API key authenticates machine calls as your business rather than as a person. You send it in the same api-key header you\n    already use for personal keys — the only difference is the APIB- prefix.\n  location: header\n  header: api-key\n  how_to_obtain: Create, rename and revoke business API keys through the management API or from the dashboard. Rotate a key by creating\
  \ a new\n    one and revoking the old one.\ndocs: https://www.eagle-doc.com/en/documentation/business-api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/eagle-doc/authentication/eagle-doc-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- OCR
- Bookkeeping
- Document-Processing
- API
---
