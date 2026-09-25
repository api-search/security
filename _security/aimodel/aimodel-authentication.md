---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aimodel-content-wp-routes-original.json
  format: json
  label: AI model Website (WordPress REST)
  slug: ai-model-jp-website-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimodel/refs/heads/main/openapi/aimodel-content-wp-routes-original.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Aimodel Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI model declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AI model
provider_slug: aimodel
scheme_count: 0
schemes: []
slug: aimodel-authentication
source_filename: aimodel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  Live probes of https://www.ai-model.jp/wp-json/ and its routes on 2026-09-14, plus the\n  `authentication` block of the WordPress route discovery document saved verbatim at\n  openapi/aimodel-content-wp-routes-original.json\nsummary: >-\n  AI model株式会社 publishes no developer program, so there is no API key, no OAuth client\n  registration and no documented authentication of any kind. Every operation captured in this repo\n  is anonymous read. The only credential scheme the host advertises is WordPress Application\n  Passwords, which is site administration for the marketing site - not a developer credential -\n  and it gates the write and administrative routes this profile deliberately excludes.\nsurfaces:\n- key: content\n  name: AI model WordPress REST API\n  base_url: https://www.ai-model.jp/wp-json\n  security_schemes: []\n  anonymous_read: true\n  verified: 'GET /wp/v2/models, /wp/v2/news, /wp/v2/pages, /wp/v2/media,\
  \ /wp/v2/categories, /wp/v2/search, /wp/v2/types, /wp/v2/taxonomies and /wp/v2/statuses each returned HTTP 200 with no credentials on 2026-09-14.'\ngated_routes:\n- path: /wp/v2/settings\n  status: 401\n  note: Site settings; requires an authenticated administrator.\n- path: /wp-abilities/v1/abilities\n  status: 401\n  note: WordPress Abilities API - registered, but not readable anonymously.\n- path: /smart-cf-api/v2/search/posts\n  status: 401\n- path: /wp/v2/block-types\n  status: 401\n- path: /contact-form-7/v1/contact-forms\n  status: 403\n  note: Contact Form 7 form definitions; the public contact form itself posts through the site UI.\napplication_passwords:\n  advertised: true\n  authorization_endpoint: https://www.ai-model.jp/wp/wp-admin/authorize-application.php\n  transport: HTTP Basic\n  note: >-\n    Advertised in the discovery document's `authentication` block. These are WordPress site\n    administration credentials issued to site editors, not an API program open to third\
  \ parties.\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\ndocs: null\ndocs_note: No authentication documentation exists because no developer documentation exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimodel/refs/heads/main/authentication/aimodel-authentication.yml
summary_line: 0 schemes
tags:
- Artificial Intelligence
- Generative AI
- Japan
- E-Commerce
- Fashion
- Apparel
- Advertising
- Marketing
- Content
- Digital Human
- Media
- WordPress
---
