---
api_key_in:
- query
auth_types:
- oauth1
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 500Px Authentication
name_suffix: Authentication
oauth_flows: []
overview: 500px secures its APIs with oauth1 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 500px
provider_slug: 500px
scheme_count: 2
schemes:
- description: Public read-only requests (feature streams, public photos, public user profiles) are signed with a Consumer Key passed as the consumer_key query-string parameter. No user context.
  in: query
  name: ConsumerKey
  parameter: consumer_key
  sources:
  - https://github.com/500px/legacy-api-documentation
  type: apiKey
- access_token_url: https://api.500px.com/v1/oauth/access_token
  authorize_url: https://api.500px.com/v1/oauth/authorize
  description: User-scoped requests (uploads, voting, following, private data) use three-legged OAuth 1.0a with HMAC-SHA1 request signing.
  flow: 1.0a
  name: OAuth1
  request_token_url: https://api.500px.com/v1/oauth/request_token
  sources:
  - https://github.com/500px/legacy-api-documentation
  type: oauth1
slug: 500px-authentication
source_filename: 500px-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://github.com/500px/legacy-api-documentation/blob/master/README.md\ndocs: https://github.com/500px/legacy-api-documentation/blob/master/authentication/README.md\nstatus: retired\nnote: >-\n  The 500px public API program was discontinued on 2018-06-15. The authentication model below is\n  captured from the legacy API documentation for historical reference; live credentials are no\n  longer issued.\nsummary:\n  types: [oauth1, apiKey]\n  api_key_in: [query]\n  oauth_version: 1.0a\nschemes:\n- name: ConsumerKey\n  type: apiKey\n  in: query\n  parameter: consumer_key\n  description: >-\n    Public read-only requests (feature streams, public photos, public user profiles) are signed\n    with a Consumer Key passed as the consumer_key query-string parameter. No user context.\n  sources: [https://github.com/500px/legacy-api-documentation]\n- name: OAuth1\n  type: oauth1\n  flow: 1.0a\n  request_token_url: https://api.500px.com/v1/oauth/request_token\n\
  \  authorize_url: https://api.500px.com/v1/oauth/authorize\n  access_token_url: https://api.500px.com/v1/oauth/access_token\n  description: >-\n    User-scoped requests (uploads, voting, following, private data) use three-legged OAuth 1.0a\n    with HMAC-SHA1 request signing.\n  sources: [https://github.com/500px/legacy-api-documentation]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/500px/refs/heads/main/authentication/500px-authentication.yml
summary_line: oauth1/apiKey · 2 schemes
tags:
- Company
- Photography
- Stock Photos
- Image Licensing
- Community
- Social Network
- Media
- Content
---
