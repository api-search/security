---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wallabag-openapi-generated.yml
  format: yaml
  label: wallabag API
  slug: wallabag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wallabag/openapi/_ae-authored/wallabag-openapi-generated.yml
auth_types: []
description: OAuth2 password grant authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wallabag Authentication
name_suffix: Authentication
oauth_flows: []
overview: wallabag declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: wallabag
provider_slug: wallabag
scheme_count: 1
schemes:
- evidence: We will use the access_token value in our subsequent API calls.
  flows:
  - password
  how_to_obtain: Create a new API client in your wallabag account to get a client_id and client_secret, then request an access token via the password grant using client_id, client_secret, username and password as shown in the documentation.
  name: OAuth2 Password Grant
  token_url: http://localhost:8000/oauth/v2/token
  type: oauth2
slug: wallabag-authentication
source_filename: wallabag-authentication.yml
source_heading: Authentication Profile
source_url: https://doc.wallabag.org/developer/api/oauth/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://doc.wallabag.org/developer/api/oauth/\nsources:\n- https://doc.wallabag.org/developer/api/oauth/\ndescription: OAuth2 password grant authentication\nschemes:\n- type: oauth2\n  name: OAuth2 Password Grant\n  evidence: We will use the access_token value in our subsequent API calls.\n  flows:\n  - password\n  token_url: http://localhost:8000/oauth/v2/token\n  how_to_obtain: Create a new API client in your wallabag account to get a client_id and client_secret, then request an access token via the password\n    grant using client_id, client_secret, username and password as shown in the documentation.\ndocs: https://doc.wallabag.org/developer/api/oauth/\n"
source_yaml_url: https://artifacts.apis.io/wallabag/authentication/wallabag-authentication.yml
summary_line: 1 scheme
tags:
- Open Source
- Read-it-later
- Self-hosted
- Privacy
- Community
---
