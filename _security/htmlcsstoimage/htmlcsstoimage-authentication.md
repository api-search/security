---
api_key_in: []
api_specs:
- filename: htmlcsstoimage-openapi.yml
  format: yaml
  label: HTML/CSS to Image Generation API
  slug: image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/htmlcsstoimage/refs/heads/main/openapi/htmlcsstoimage-openapi.yml
- filename: htmlcsstoimage-openapi.yml
  format: yaml
  label: HTML/CSS to Image Templates API
  slug: templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/htmlcsstoimage/refs/heads/main/openapi/htmlcsstoimage-openapi.yml
- filename: htmlcsstoimage-openapi.yml
  format: yaml
  label: HTML/CSS to Image Signed URLs API
  slug: signed-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/htmlcsstoimage/refs/heads/main/openapi/htmlcsstoimage-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Htmlcsstoimage Authentication
name_suffix: Authentication
oauth_flows: []
overview: HTML/CSS to Image secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HTML/CSS to Image
provider_slug: htmlcsstoimage
scheme_count: 1
schemes:
- description: HTTP Basic authentication using your User ID as the username and your API Key as the password, both from the HTML/CSS to Image dashboard.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/htmlcsstoimage-openapi.yml
  type: http
slug: htmlcsstoimage-authentication
source_filename: htmlcsstoimage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/htmlcsstoimage-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your User ID as the username and your API Key\n    as the password, both from the HTML/CSS to Image dashboard.\n  sources:\n  - openapi/htmlcsstoimage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/htmlcsstoimage/refs/heads/main/authentication/htmlcsstoimage-authentication.yml
summary_line: http · 1 scheme
tags:
- Image Generation
- HTML to Image
- CSS to Image
- Rendering
- Screenshots
- Templates
---
