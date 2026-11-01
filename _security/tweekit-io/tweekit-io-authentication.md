---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses API key and secret passed as HTTP headers.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tweekit Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: tweekit-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: tweekit-io
provider_slug: tweekit-io
scheme_count: 2
schemes:
- evidence: Note that the TweekIT API expects the API key header names to be "apikey" and "apisecret" instead of "x-api-key" and "secret-api-key" respectively to allow compatibility with certain Javascript libraries which do not work with header names that contain dashes when doing HTTP requests.
  header: apikey
  location: header
  name: apikey
  type: apiKey
- evidence: Note that the TweekIT API expects the API key header names to be "apikey" and "apisecret" instead of "x-api-key" and "secret-api-key" respectively to allow compatibility with certain Javascript libraries which do not work with header names that contain dashes when doing HTTP requests.
  header: apisecret
  location: header
  name: apisecret
  type: apiKey
slug: tweekit-io-authentication
source_filename: tweekit-io-authentication.yml
source_heading: Authentication Profile
source_url: https://tweekit.io/docs/authentication/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tweekit.io/docs/authentication/\nsources:\n- https://tweekit.io/docs/authentication/\n- https://tweekit.io/docs/using-api-keys/\ndescription: Authentication uses API key and secret passed as HTTP headers.\nschemes:\n- type: apiKey\n  name: apikey\n  evidence: Note that the TweekIT API expects the API key header names to be \"apikey\" and \"apisecret\" instead of \"x-api-key\" and \"secret-api-key\"\n    respectively to allow compatibility with certain Javascript libraries which do not work with header names that contain dashes when doing HTTP\n    requests.\n  location: header\n  header: apikey\n- type: apiKey\n  name: apisecret\n  evidence: Note that the TweekIT API expects the API key header names to be \"apikey\" and \"apisecret\" instead of \"x-api-key\" and \"secret-api-key\"\n    respectively to allow compatibility with certain Javascript libraries which do not work\
  \ with header names that contain dashes when doing HTTP\n    requests.\n  location: header\n  header: apisecret\nnote: Both headers must be included in each request.\ndocs: https://tweekit.io/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/tweekit-io/authentication/tweekit-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- File-Conversion
- API
- Media
---
