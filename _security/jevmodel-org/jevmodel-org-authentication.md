---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jevmodel-org-openapi-generated.yml
  format: yaml
  label: Jev Model Guide API
  slug: jevmodel-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jevmodel-org/openapi/_ae-authored/jevmodel-org-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jevmodel Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jev Model Guide declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jev Model Guide
provider_slug: jevmodel-org
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer $JEVMODEL_API_KEY'
  header: Authorization
  how_to_obtain: Create an API key in the jevmodel.org Dashboard and save it as JEVMODEL_API_KEY.
  location: header
  name: Bearer
  type: http-bearer
slug: jevmodel-org-authentication
source_filename: jevmodel-org-authentication.yml
source_heading: Authentication Profile
source_url: https://jevmodel.org/dashboard/
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://jevmodel.org/dashboard/\nsources:\n- https://jevmodel.org/dashboard/\n- https://jevmodel.org/how-to-use-jev/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer $JEVMODEL_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the jevmodel.org Dashboard and save it as JEVMODEL_API_KEY.\ndocs: https://jevmodel.org/dashboard/\n"
source_yaml_url: https://artifacts.apis.io/jevmodel-org/authentication/jevmodel-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Decision-Model
- API
- TypeSafe
---
