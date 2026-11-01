---
anonymous_access: false
api_key_in: []
auth_types: []
description: Redditapis uses a simple API key that is sent as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Redditapis Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: redditapis-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: redditapis-com
provider_slug: redditapis-com
scheme_count: 1
schemes:
- evidence: Sign up for a Redditapis key, then send a GET request to api.redditapis.com with an Authorization header set to Bearer YOUR_API_KEY.
  header: Authorization
  how_to_obtain: Sign up at redditapis.com; the bearer token is issued immediately and can be copied from the dashboard.
  location: header
  name: API Key
  type: http-bearer
slug: redditapis-com-authentication
source_filename: redditapis-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.redditapis.com/reddit-api-key
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.redditapis.com/reddit-api-key\nsources:\n- https://www.redditapis.com/reddit-api-key\n- https://www.redditapis.com/quickstart\ndescription: Redditapis uses a simple API key that is sent as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Sign up for a Redditapis key, then send a GET request to api.redditapis.com with an Authorization header set to Bearer YOUR_API_KEY.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at redditapis.com; the bearer token is issued immediately and can be copied from the dashboard.\nnote: No OAuth2 flows or other authentication schemes are described on the referenced pages.\ndocs: https://www.redditapis.com/reddit-api-key\n"
source_yaml_url: https://artifacts.apis.io/redditapis-com/authentication/redditapis-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Reddit
- Pay-per-call
- AI
---
