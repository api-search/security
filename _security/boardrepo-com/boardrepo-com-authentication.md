---
anonymous_access: false
api_key_in: []
api_specs:
- filename: boardrepo-com-openapi-generated.yml
  format: yaml
  label: BoardRepo API
  slug: boardrepo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardrepo-com/openapi/_ae-authored/boardrepo-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Boardrepo Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BoardRepo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BoardRepo
provider_slug: boardrepo-com
scheme_count: 1
schemes:
- authorize_url: https://boardrepo.com/oauth/authorize
  evidence: Auth is OAuth via dynamic client registration, so there is no API key or secret to set.
  flows:
  - authorization_code
  how_to_obtain: dynamic client registration
  name: OAuth
  scopes:
  - read:public
  type: oauth2
slug: boardrepo-com-authentication
source_filename: boardrepo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://boardrepo.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://boardrepo.com/.well-known/oauth-protected-resource\nsources:\n- https://boardrepo.com/.well-known/oauth-protected-resource\n- https://boardrepo.com/.well-known/oauth-authorization-server\n- https://boardrepo.com/connect\n- https://boardrepo.com/contact?plan=team\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Auth is OAuth via dynamic client registration, so there is no API key or secret to set.\n  flows:\n  - authorization_code\n  authorize_url: https://boardrepo.com/oauth/authorize\n  scopes:\n  - read:public\n  how_to_obtain: dynamic client registration\ndocs: https://boardrepo.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/boardrepo-com/authentication/boardrepo-com-authentication.yml
summary_line: 1 scheme
tags:
- Hardware
- KiCad
- Collaboration
- Open Source
- Design
---
