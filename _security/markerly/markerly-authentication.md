---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Markerly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Markerly declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Markerly
provider_slug: markerly
scheme_count: 0
schemes: []
slug: markerly-authentication
source_filename: markerly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Live probes of https://media-processor-65la52ndha-uc.a.run.app,\n  https://api.markerly.com/, and https://markerly.creatorsaurus.com/ on\n  2026-08-12, plus Markerly's published source at\n  https://github.com/Markerly/media-processor-microservice.\nnotes: >-\n  Markerly issues no API keys and publishes no developer authentication\n  documentation. There are three distinct authentication postures across its\n  surfaces, and only one of them belongs to a callable API.\n\nsurfaces:\n\n- name: Media Processor microservice\n  api: markerly:media-processor\n  base_url: https://media-processor-65la52ndha-uc.a.run.app\n  authenticated: false\n  scheme: none\n  evidence:\n    url: https://media-processor-65la52ndha-uc.a.run.app/\n    http_status: 200\n    note: >-\n      Returned its full service-discovery document to an anonymous request with\n      no credential of any kind. GET /health likewise returns 200 anonymously.\n  controls_in_place:\n\
  \  - Per-IP rate limiting (100 requests / 15 minutes) as the only abuse control.\n  - >-\n      Input allow-listing: POST /generate-thumbnail refuses any videoUrl that is\n      not a Google Cloud Storage URL with a video file extension, which bounds\n      the SSRF surface in the absence of authentication.\n  - helmet security headers and HSTS (max-age 15552000; includeSubDomains).\n  concerns:\n  - >-\n      CORS is wide open (access-control-allow-origin: *) on an unauthenticated\n      endpoint that performs resource-intensive FFmpeg work, so any origin can\n      drive it from a browser.\n  - >-\n      The source comments describe this as an \"internal microservice\", but it is\n      reachable from the public internet without credentials. If it is meant to\n      be internal, Cloud Run IAM or an ingress restriction — not just a rate\n      limiter — is the missing control.\n\n- name: Creator social-connect app\n  host: https://api.markerly.com\n  authenticated: true\n  audience: creators\
  \ (Markerly's influencer network), not developers\n  schemes:\n  - type: form-login\n    detail: Email + password POST to /login with a Laravel CSRF token.\n  - type: oauth2\n    provider: Facebook / Meta\n    detail: >-\n      Facebook JS SDK login (Graph API v25.0) requesting scopes public_profile,\n      email, instagram_basic, instagram_manage_insights, pages_read_engagement,\n      pages_show_list — i.e. creators grant Markerly read access to their\n      Instagram insights and Facebook Page engagement.\n    posted_to: https://api.markerly.com/facebook/login\n  - type: oauth2\n    provider: TikTok\n    posted_to: https://api.markerly.com/tiktok/login\n  password_reset: https://api.markerly.com/password/reset\n  evidence:\n    url: https://api.markerly.com/\n    http_status: 200\n  note: >-\n    Despite the api.* hostname this is a Laravel web application serving an HTML\n    login page, not a machine API. No OpenAPI, no token endpoint, and no\n    /.well-known/oauth-authorization-server\
  \ (probed, 404).\n\n- name: Creator / client platform portal\n  host: https://markerly.creatorsaurus.com\n  authenticated: true\n  scheme: form-login (JavaScript-rendered single-page application)\n  sign_up: https://markerly.creatorsaurus.com/register\n  sign_in: https://markerly.creatorsaurus.com/login\n  evidence:\n    url: https://markerly.creatorsaurus.com/login\n    http_status: 200\n  note: >-\n    Markerly's platform is served from the creatorsaurus.com domain under a\n    markerly.* tenant subdomain; the apex creatorsaurus.com itself returns a\n    page titled \"Markerly\". The portal is a Vue SPA whose served HTML is an\n    empty shell, so nothing behind it is machine-readable.\n\nwell_known:\n  oauth_authorization_server: 404 on markerly.com, api.markerly.com, and the Cloud Run host\n  openid_configuration: 404 on markerly.com, api.markerly.com, and the Cloud Run host\n  oauth_protected_resource: 404 on api.markerly.com\n\noauth_scopes_artifact: >-\n  Not applicable. Markerly\
  \ is an OAuth *client* of Meta and TikTok, not an OAuth\n  provider — it publishes no authorization server and no scope reference, so\n  scopes/ is intentionally absent rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markerly/refs/heads/main/authentication/markerly-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Influencer Marketing
- Marketing
- Creator Economy
- Advertising
- Social-Media
- Advocacy
- Media Processing
- Public Sector
---
