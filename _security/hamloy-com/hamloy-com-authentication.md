---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hamloy-com-openapi-generated.yml
  format: yaml
  label: Hamloy API
  slug: hamloy-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamloy-com/openapi/_ae-authored/hamloy-com-openapi-generated.yml
auth_types: []
description: Clients authenticate to Hamloy either via an API token sent as a Bearer token in the Authorization header, or via an OAuth sign‑in flow that returns a temporary key (details not published).
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hamloy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hamloy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hamloy
provider_slug: hamloy-com
scheme_count: 2
schemes:
- evidence: 'An agent sends the token in a header with every call:


    ```

    Authorization: Bearer hml_…

    ```'
  header: Authorization
  how_to_obtain: Create a token on the Connect page under API tokens; it starts with `hml_` and is shown once.
  location: header
  name: API token
  type: http-bearer
- evidence: Sign in (OAuth). Give the app the address and nothing else. The first time it calls, Hamloy answers that it needs a sign‑in, and says where. The app opens hamloy.com in your browser, you sign in and choose **Allow** , and the app keeps the key it gets back.
  how_to_obtain: The app initiates sign‑in; Hamloy redirects to a browser where the user signs in and authorizes, returning a temporary key.
  name: Sign in (OAuth)
  type: oauth2
slug: hamloy-com-authentication
source_filename: hamloy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://hamloy.com/docs/sign-in.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hamloy.com/docs/sign-in.md\nsources:\n- https://hamloy.com/docs/sign-in.md\n- https://hamloy.com/docs/api-tokens.md\n- https://hamloy.com/docs/usage.md\n- https://hamloy.com/docs/remote-link-or-token.md\ndescription: Clients authenticate to Hamloy either via an API token sent as a Bearer token in the Authorization header, or via an OAuth sign‑in\n  flow that returns a temporary key (details not published).\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: 'An agent sends the token in a header with every call:\n\n\n    ```\n\n    Authorization: Bearer hml_…\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token on the Connect page under API tokens; it starts with `hml_` and is shown once.\n- type: oauth2\n  name: Sign in (OAuth)\n  evidence: Sign in (OAuth). Give the app the address and nothing else. The first time it calls,\
  \ Hamloy answers that it needs a sign‑in, and says\n    where. The app opens hamloy.com in your browser, you sign in and choose **Allow** , and the app keeps the key it gets back.\n  how_to_obtain: The app initiates sign‑in; Hamloy redirects to a browser where the user signs in and authorizes, returning a temporary key.\ndocs: https://hamloy.com/docs/sign-in.md\n"
source_yaml_url: https://artifacts.apis.io/hamloy-com/authentication/hamloy-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
