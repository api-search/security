---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allwhere-beta-api-openapi.yml
  format: yaml
  label: allwhere Beta API
  slug: allwhere-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allwhere/refs/heads/main/openapi/allwhere-beta-api-openapi.yml
auth_types: []
description: Authentication schemes for allwhere API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Allwhere Authentication
name_suffix: Authentication
oauth_flows: []
overview: allwhere declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: allwhere
provider_slug: allwhere
scheme_count: 1
schemes:
- evidence: All API requests require authentication using an API key passed in the `Authorization` header as a Bearer token.
  header: Authorization
  how_to_obtain: https://app.allwhere.co/integrations/api-access
  location: header
  name: Bearer
  type: http-bearer
slug: allwhere-authentication
source_filename: allwhere-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.allwhere.co/docs/getting-started.md
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.allwhere.co/docs/getting-started.md\nsources:\n- https://docs.allwhere.co/docs/getting-started.md\n- https://docs.allwhere.co/docs/quick-start-guide.md\ndescription: Authentication schemes for allwhere API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All API requests require authentication using an API key passed in the `Authorization` header as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: https://app.allwhere.co/integrations/api-access\ndocs: https://docs.allwhere.co/docs/getting-started.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allwhere/refs/heads/main/authentication/allwhere-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IT
- Asset-Management
- Procurement
- Remote-Workforce
- Enterprise
---
