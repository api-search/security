---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bmlt-app-openapi-generated.yml
  format: yaml
  label: BMLT.app API
  slug: bmlt-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bmlt-app/openapi/_ae-authored/bmlt-app-openapi-generated.yml
auth_types: []
description: Authentication is performed by obtaining a bearer token via the /api/v1/auth/token endpoint and then sending it in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BMLT.app Authentication
name_suffix: Authentication
oauth_flows: []
overview: BMLT.app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BMLT.app
provider_slug: bmlt-app
scheme_count: 1
schemes:
- evidence: Creates a token
  header: Authorization
  how_to_obtain: POST /api/v1/auth/token with a JSON body containing "username" and "password" fields.
  location: header
  name: Bearer
  token_url: /api/v1/auth/token
  type: http-bearer
slug: bmlt-app-authentication
source_filename: bmlt-app-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.bmlt.app/#/rootServer/authToken
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.bmlt.app/#/rootServer/authToken\nsources:\n- https://api-docs.bmlt.app/#/rootServer/authToken\n- https://api-docs.bmlt.app/#/rootServer/authRefresh\n- https://api-docs.bmlt.app/#/rootServer/authLogout\ndescription: Authentication is performed by obtaining a bearer token via the /api/v1/auth/token endpoint and then sending it in the Authorization\n  header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Creates a token\n  location: header\n  header: Authorization\n  token_url: /api/v1/auth/token\n  how_to_obtain: POST /api/v1/auth/token with a JSON body containing \"username\" and \"password\" fields.\ndocs: https://api-docs.bmlt.app/#/rootServer/authToken\n"
source_yaml_url: https://artifacts.apis.io/bmlt-app/authentication/bmlt-app-authentication.yml
summary_line: 1 scheme
tags:
- Open Source
- Narcotics Anonymous
- Meeting Management
- Community
- BMLT
---
