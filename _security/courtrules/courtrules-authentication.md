---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Court Rules API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Courtrules Authentication
name_suffix: Authentication
oauth_flows: []
overview: Court Rules declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Court Rules
provider_slug: courtrules
scheme_count: 1
schemes:
- evidence: All API endpoints require a Bearer token in the `Authorization` header.
  header: Authorization
  how_to_obtain: API keys are issued through the console dashboard at console.courtrules.app; the key is used as a Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: courtrules-authentication
source_filename: courtrules-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.courtrules.app/authentication.md
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.courtrules.app/authentication.md\nsources:\n- https://docs.courtrules.app/authentication.md\n- https://docs.courtrules.app/quickstart.md\ndescription: Authentication methods for Court Rules API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: All API endpoints require a Bearer token in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are issued through the console dashboard at console.courtrules.app; the key is used as a Bearer token.\ndocs: https://docs.courtrules.app/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courtrules/refs/heads/main/authentication/courtrules-authentication.yml
summary_line: 1 scheme
tags:
- LegalData
- API
- CourtRules
- Compliance
- USLaw
---
