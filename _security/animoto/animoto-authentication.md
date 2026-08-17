---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Animoto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Animoto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Animoto
provider_slug: animoto
scheme_count: 1
schemes:
- description: HTTP Basic authentication over TLS. Credentials are an Animoto platform key (username) and platform secret (password), issued to partners. There is no public self-service route to obtain them — see lifecycle/animoto-lifecycle.yml.
  name: basicAuth
  realm: Application
  scheme: basic
  sources:
  - probe:https://api.animoto.com/jobs/
  - https://rubygems.org/gems/animoto
  - https://github.com/animoto/animoto_api_sample_app_ruby
  type: http
slug: animoto-authentication
source_filename: animoto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.animoto.com/jobs/\nnote: >-\n  No OpenAPI or Swagger definition exists in this repo and Animoto publishes no public\n  authentication documentation, so this profile was established by PROBING the live API host\n  rather than derived from a spec. Every path requested on api.animoto.com returns\n  `HTTP/2 401` with `www-authenticate: Basic realm=\"Application\"` and the body\n  `HTTP Basic: Access denied.` That is a directly observed authentication challenge, not an\n  inference. It is corroborated by Animoto's own first-party code: the `animoto` RubyGem\n  (published by Animoto) constructs its client as `Animoto::Client.new(key, secret)` and the\n  first-party sample app animoto/animoto_api_sample_app_ruby passes\n  `ANIMOTO_PLATFORM_USERNAME` / `ANIMOTO_PLATFORM_PASSWORD` into that constructor — an\n  Animoto platform key + secret carried as HTTP Basic credentials.\nsummary:\n  types:\n  - http\n  http_schemes:\n\
  \  - basic\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mtls: false\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  realm: Application\n  description: >-\n    HTTP Basic authentication over TLS. Credentials are an Animoto platform key (username) and\n    platform secret (password), issued to partners. There is no public self-service route to\n    obtain them — see lifecycle/animoto-lifecycle.yml.\n  sources:\n  - probe:https://api.animoto.com/jobs/\n  - https://rubygems.org/gems/animoto\n  - https://github.com/animoto/animoto_api_sample_app_ruby\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://api.animoto.com/jobs/\n  http_status: 401\n  www_authenticate: 'Basic realm=\"Application\"'\n  body: 'HTTP Basic: Access denied.'\n  server_headers:\n    strict-transport-security: max-age=15724800; includeSubDomains\n    x-animoto-request-id: present\n    x-served-by: ingress-nginx-controller\ngaps:\n- No published authentication documentation on\
  \ any Animoto host.\n- No OAuth 2.0, OpenID Connect, or scope surface observed or documented.\n- >-\n  Token/credential lifecycle (rotation, revocation, expiry) is undocumented publicly and could\n  not be probed anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/animoto/refs/heads/main/authentication/animoto-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Video
- Video Creation
- Video Editing
- Slideshow
- Marketing
- Social Media
- Content Creation
- SaaS
---
