---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kapost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kapost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kapost
provider_slug: kapost
scheme_count: 1
schemes:
- description: 'Basic auth where the API token is supplied as the username and the password is disregarded. Example: curl -u "token:x" "https://your_instance.kapost.com/api/v1/content"'
  name: basicAuth
  scheme: basic
  source: https://developer.kapost.com/api-getting-started
  sources:
  - https://developer.kapost.com/api-getting-started
  type: http
slug: kapost-authentication
source_filename: kapost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.kapost.com/api-getting-started\ndocs: https://developer.kapost.com/api-getting-started\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  notes: >-\n    HTTP Basic authentication. The username is a per-user API token obtained\n    from the user's edit-profile page in the Kapost instance; the password is\n    ignored (any value, e.g. \"x\"). All API actions appear to originate from the\n    account that owns the token. There is no OAuth 2.0 / OpenID Connect surface.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Basic auth where the API token is supplied as the username and the\n      password is disregarded. Example:\n      curl -u \"token:x\" \"https://your_instance.kapost.com/api/v1/content\"\n    source: https://developer.kapost.com/api-getting-started\n    sources: [https://developer.kapost.com/api-getting-started]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kapost/refs/heads/main/authentication/kapost-authentication.yml
summary_line: http · 1 scheme
tags:
- Content Operations
- Content Marketing
- Content Management
- Marketing
- Sales Enablement
- Webhooks
- REST API
- B2B
- Upland Software
---
