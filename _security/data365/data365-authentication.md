---
anonymous_access: false
api_key_in: []
auth_types: []
description: Reddit uses OAuth 2.0 for authentication. Clients must register an app to obtain a Client ID and Client Secret, then exchange them for an OAuth access token which is sent in the Authorization header as a Bearer token. A descriptive User-Agent header is also required.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Data365 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Data365 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Data365
provider_slug: data365
scheme_count: 1
schemes:
- evidence: The official tool requires OAuth for authenticated requests; traffic not using OAuth or Reddit API login credentials will be blocked.
  how_to_obtain: Register an app in Reddit account settings to receive a Client ID and Client Secret, then use them to obtain an OAuth access token.
  name: Reddit OAuth2
  type: oauth2
slug: data365-authentication
source_filename: data365-authentication.yml
source_heading: Authentication Profile
source_url: https://data365.co/blog/how-to-get-reddit-api-key
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://data365.co/blog/how-to-get-reddit-api-key\nsources:\n- https://data365.co/blog/how-to-get-reddit-api-key\ndescription: Reddit uses OAuth 2.0 for authentication. Clients must register an app to obtain a Client ID and Client Secret, then exchange them\n  for an OAuth access token which is sent in the Authorization header as a Bearer token. A descriptive User-Agent header is also required.\nschemes:\n- type: oauth2\n  name: Reddit OAuth2\n  evidence: The official tool requires OAuth for authenticated requests; traffic not using OAuth or Reddit API login credentials will be blocked.\n  how_to_obtain: Register an app in Reddit account settings to receive a Client ID and Client Secret, then use them to obtain an OAuth access\n    token.\ndocs: https://data365.co/blog/how-to-get-reddit-api-key\n"
source_yaml_url: https://artifacts.apis.io/data365/authentication/data365-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- Real-Time Data
- Developers
---
