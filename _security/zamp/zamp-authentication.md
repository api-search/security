---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zamp-openapi-generated.yml
  format: yaml
  label: Zamp API
  slug: zamp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zamp/refs/heads/main/openapi/_ae-authored/zamp-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Zamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zamp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Zamp
provider_slug: zamp
scheme_count: 1
schemes:
- evidence: All API calls require the key in the HTTP `Authorization` header.
  header: Authorization
  how_to_obtain: Get a free 30‑day trial key or copy your production key from your Zamp account.
  location: header
  name: Bearer
  type: http-bearer
slug: zamp-authentication
source_filename: zamp-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.zamp.com/guides/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.zamp.com/guides/authentication.md\nsources:\n- https://developer.zamp.com/guides/authentication.md\n- https://developer.zamp.com/guides/quickstart.md\n- https://developer.zamp.com/big-commerce-getting-started.md\n- https://developer.zamp.com/adobe-commerce-getting-started.md\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All API calls require the key in the HTTP `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: Get a free 30‑day trial key or copy your production key from your Zamp account.\ndocs: https://developer.zamp.com/guides/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zamp/refs/heads/main/authentication/zamp-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SalesTax
- API
- Automation
- Compliance
---
