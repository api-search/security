---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trip2g-com-openapi-generated.yml
  format: yaml
  label: trip2g API
  slug: trip2g-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trip2g-com/openapi/_ae-authored/trip2g-com-openapi-generated.yml
auth_types: []
description: OAuth sign‑in with Google or GitHub
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: trip2g Authentication
name_suffix: Authentication
oauth_flows: []
overview: trip2g declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: trip2g
provider_slug: trip2g-com
scheme_count: 2
schemes:
- authorize_url: /_system/auth/google?redirect=/path
  evidence: GET /_system/auth/google?redirect=/path Start Google OAuth
  flows:
  - authorization_code
  how_to_obtain: Register an application in Google Cloud Console, add the redirect URI https://your-domain.com/_system/auth/google/callback, copy the Client ID and Client Secret, and enter them in the Trip2G admin panel.
  name: Google
  type: oauth2
- authorize_url: /_system/auth/github?redirect=/path
  evidence: GET /_system/auth/github?redirect=/path Start GitHub OAuth
  flows:
  - authorization_code
  how_to_obtain: Create a new OAuth App in GitHub Developer Settings, set the Authorization callback URL to https://your-domain.com/_system/auth/github/callback, copy the Client ID and Client Secret, and enter them in the Trip2G admin panel.
  name: GitHub
  type: oauth2
slug: trip2g-com-authentication
source_filename: trip2g-com-authentication.yml
source_heading: Authentication Profile
source_url: https://trip2g.com/en/user/oauth
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://trip2g.com/en/user/oauth\nsources:\n- https://trip2g.com/en/user/oauth\n- https://trip2g.com/ru/user/oauth\n- https://trip2g.com/dev/2026_07_02_vector_search_token_economy\n- https://trip2g.com/dev/google_github_auth\ndescription: OAuth sign‑in with Google or GitHub\nschemes:\n- type: oauth2\n  name: Google\n  evidence: GET /_system/auth/google?redirect=/path Start Google OAuth\n  flows:\n  - authorization_code\n  authorize_url: /_system/auth/google?redirect=/path\n  how_to_obtain: Register an application in Google Cloud Console, add the redirect URI https://your-domain.com/_system/auth/google/callback, copy\n    the Client ID and Client Secret, and enter them in the Trip2G admin panel.\n- type: oauth2\n  name: GitHub\n  evidence: GET /_system/auth/github?redirect=/path Start GitHub OAuth\n  flows:\n  - authorization_code\n  authorize_url: /_system/auth/github?redirect=/path\n\
  \  how_to_obtain: Create a new OAuth App in GitHub Developer Settings, set the Authorization callback URL to https://your-domain.com/_system/auth/github/callback,\n    copy the Client ID and Client Secret, and enter them in the Trip2G admin panel.\ndocs: https://trip2g.com/en/user/oauth\n"
source_yaml_url: https://artifacts.apis.io/trip2g-com/authentication/trip2g-com-authentication.yml
summary_line: 2 schemes
tags:
- Knowledge
- OpenSource
- AI
- SelfHosted
- Markdown
---
