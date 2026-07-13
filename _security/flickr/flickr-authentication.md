---
api_key_in:
- query
api_specs:
- filename: flickr-openapi.yml
  format: yaml
  label: Flickr API
  slug: flickr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flickr/refs/heads/main/openapi/flickr-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Flickr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Flickr secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Flickr
provider_slug: flickr
scheme_count: 2
schemes:
- description: Application API key for non-authenticated and read-only public requests.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/flickr-openapi.yml
  type: apiKey
- description: 'Flickr uses OAuth 1.0a (HMAC-SHA1). The OpenAPI 3 schema cannot model

    OAuth 1.0a directly, so this entry approximates the flow. Token URLs:

    - Request token: https://www.flickr.com/services/oauth/request_token

    - Authorize:     https://www.flickr.com/services/oauth/authorize

    - Access token:  https://www.flickr.com/services/oauth/access_token'
  flows:
  - authorizationUrl: https://www.flickr.com/services/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://www.flickr.com/services/oauth/access_token
  name: OAuth1
  sources:
  - openapi/flickr-openapi.yml
  type: oauth2
slug: flickr-authentication
source_filename: flickr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flickr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Application API key for non-authenticated and read-only public requests.\n  sources:\n  - openapi/flickr-openapi.yml\n- name: OAuth1\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.flickr.com/services/oauth/authorize\n    tokenUrl: https://www.flickr.com/services/oauth/access_token\n    scopes: 3\n  description: |-\n    Flickr uses OAuth 1.0a (HMAC-SHA1). The OpenAPI 3 schema cannot model\n    OAuth 1.0a directly, so this entry approximates the flow. Token URLs:\n    - Request token: https://www.flickr.com/services/oauth/request_token\n    - Authorize:     https://www.flickr.com/services/oauth/authorize\n    - Access token:  https://www.flickr.com/services/oauth/access_token\n\
  \  sources:\n  - openapi/flickr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flickr/refs/heads/main/authentication/flickr-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Photography
- Photos
- Social Media
- Public APIs
---
