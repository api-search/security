---
api_key_in: []
api_specs:
- filename: shutterstock-audio-api-openapi.yml
  format: yaml
  label: Shutterstock audio API
  slug: shutterstock-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-audio-api-openapi.yml
- filename: shutterstock-computer-vision-api-openapi.yml
  format: yaml
  label: Shutterstock computer_vision API
  slug: shutterstock-computer-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-computer-vision-api-openapi.yml
- filename: shutterstock-contributors-api-openapi.yml
  format: yaml
  label: Shutterstock contributors API
  slug: shutterstock-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-contributors-api-openapi.yml
- filename: shutterstock-editorial-images-api-openapi.yml
  format: yaml
  label: Shutterstock editorial_images API
  slug: shutterstock-editorial-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-editorial-images-api-openapi.yml
- filename: shutterstock-editorial-video-api-openapi.yml
  format: yaml
  label: Shutterstock editorial_video API
  slug: shutterstock-editorial-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-editorial-video-api-openapi.yml
- filename: shutterstock-images-api-openapi.yml
  format: yaml
  label: Shutterstock images API
  slug: shutterstock-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-images-api-openapi.yml
- filename: shutterstock-oauth-api-openapi.yml
  format: yaml
  label: Shutterstock oauth API
  slug: shutterstock-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-oauth-api-openapi.yml
- filename: shutterstock-test-api-openapi.yml
  format: yaml
  label: Shutterstock test API
  slug: shutterstock-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-test-api-openapi.yml
- filename: shutterstock-users-api-openapi.yml
  format: yaml
  label: Shutterstock users API
  slug: shutterstock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-users-api-openapi.yml
- filename: shutterstock-videos-api-openapi.yml
  format: yaml
  label: Shutterstock videos API
  slug: shutterstock-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/openapi/shutterstock-videos-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Shutterstock Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Shutterstock secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Shutterstock
provider_slug: shutterstock
scheme_count: 2
schemes:
- name: basic
  scheme: basic
  sources:
  - openapi/shutterstock-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://accounts.shutterstock.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://api.shutterstock.com/v2/oauth/access_token
  name: customer_accessCode
  sources:
  - openapi/shutterstock-openapi.yml
  type: oauth2
slug: shutterstock-authentication
source_filename: shutterstock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shutterstock-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/shutterstock-openapi.yml\n- name: customer_accessCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.shutterstock.com/oauth/authorize\n    tokenUrl: https://api.shutterstock.com/v2/oauth/access_token\n    scopes: 5\n  sources:\n  - openapi/shutterstock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/authentication/shutterstock-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Image
- Media
- Photos
- Stock Images
- Videos
- Audio
- Licensing
- Creative Content
---
