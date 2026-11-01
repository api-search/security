---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for SmugMug API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Smugmug Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmugMug declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SmugMug
provider_slug: smugmug
scheme_count: 2
schemes:
- evidence: You must include your API key in every such request. Just add APIKey=your-key-here to the query string of each request URL.
  how_to_obtain: Log in and fill out the simple form to request an API key.
  location: query
  name: APIKey
  type: apiKey
- authorize_url: https://secure.smugmug.com/services/oauth/1.0a/authorize
  evidence: We highly recommend that you use OAuth 1.0a.
  header: Authorization
  how_to_obtain: Obtain a request token via the getRequestToken endpoint, have the user authorize, then exchange for an access token.
  location: header
  name: OAuth 1.0a
  token_url: https://secure.smugmug.com/services/oauth/1.0a/getAccessToken
  type: other
slug: smugmug-authentication
source_filename: smugmug-authentication.yml
source_heading: Authentication Profile
source_url: https://api.smugmug.com/api/v2/doc/tutorial/api-key.html
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.smugmug.com/api/v2/doc/tutorial/api-key.html\nsources:\n- https://api.smugmug.com/api/v2/doc/tutorial/api-key.html\n- https://api.smugmug.com/api/v2/doc/tutorial/oauth/faq.html\n- https://api.smugmug.com/api/v2/doc/tutorial/oauth/web.html\n- https://api.smugmug.com/api/v2/doc/tutorial/oauth/non-web.html\ndescription: Authentication methods for SmugMug API\nschemes:\n- type: apiKey\n  name: APIKey\n  evidence: You must include your API key in every such request. Just add APIKey=your-key-here to the query string of each request URL.\n  location: query\n  how_to_obtain: Log in and fill out the simple form to request an API key.\n- type: other\n  name: OAuth 1.0a\n  evidence: We highly recommend that you use OAuth 1.0a.\n  location: header\n  header: Authorization\n  token_url: https://secure.smugmug.com/services/oauth/1.0a/getAccessToken\n  authorize_url: https://secure.smugmug.com/services/oauth/1.0a/authorize\n\
  \  how_to_obtain: Obtain a request token via the getRequestToken endpoint, have the user authorize, then exchange for an access token.\nnote: OAuth flows use request token, user authorization, and access token endpoints as defined in the example code.\ndocs: https://api.smugmug.com/api/v2/doc/tutorial/api-key.html\n"
source_yaml_url: https://artifacts.apis.io/smugmug/authentication/smugmug-authentication.yml
summary_line: 2 schemes
tags:
- Photography
- PhotoSharing
- ECommerce
- CloudStorage
- SaaS
---
