---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Skydance Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skydance Media secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Skydance Media
provider_slug: skydance-media
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. Read operations on wp/v2 are anonymous; every write requires credentials issued from the skydance.com WordPress admin.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/skydance-media-content-openapi.yml
  type: http
slug: skydance-media-authentication
source_filename: skydance-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/skydance-media-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Read operations on wp/v2 are\n    anonymous; every write requires credentials issued from the skydance.com WordPress admin.\n  sources:\n  - openapi/skydance-media-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydance-media/refs/heads/main/authentication/skydance-media-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Entertainment
- Media
- Film
- Television
- Animation
- Video Games
- Sports
- Content
- WordPress
---
