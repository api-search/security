---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'Authentication profile for the SynSense Website Content API. Read from the `authentication` block of the live route index and confirmed by probing the surface anonymously on 2026-09-14. The derived OpenAPI declares no securitySchemes because the described surface genuinely needs none: every content collection returns 200 to an unauthenticated GET.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Aictx Authentication
name_suffix: Authentication
oauth_flows: []
overview: aiCTX (now SynSense) declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: aiCTX (now SynSense)
provider_slug: aictx
scheme_count: 3
schemes:
- applies_to: 'All GET operations in openapi/aictx-website-content-api-openapi.json (40 of 40). The derived document sets `security: []` on every operation to state this explicitly.'
  id: none
  note: WordPress serves the `view` context of public post types to anonymous callers. The `edit` context is refused with 401 rest_forbidden_context.
  type: none
- applies_to: The write surface (POST/PUT/PATCH/DELETE) and any `context=edit` read. Not described in the derived OpenAPI, because it was never exercised and no SynSense documentation covers it.
  authorization_endpoint: https://www.synsense.ai/wp-admin/authorize-application.php
  id: application-passwords
  note: WordPress application passwords are sent as HTTP Basic (username + generated password). This is site-administrator credentialing, not a developer program — SynSense issues no API keys and publishes no onboarding path for it.
  scheme: basic
  source: 'The `authentication` object in the live route index: {"application-passwords":{"endpoints":{"authorization":"https://www.synsense.ai/wp-admin/authorize-application.php"}}}'
  type: http
- applies_to: Browser sessions inside the site's own admin/editor.
  id: cookie-nonce
  in: header
  name: X-WP-Nonce
  source: 'Advertised by the live response header `access-control-allow-headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`.'
  type: apiKey
slug: aictx-authentication
source_filename: aictx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://www.synsense.ai/wp-json/\ndescription: >-\n  Authentication profile for the SynSense Website Content API. Read from the `authentication`\n  block of the live route index and confirmed by probing the surface anonymously on 2026-09-14.\n  The derived OpenAPI declares no securitySchemes because the described surface genuinely needs\n  none: every content collection returns 200 to an unauthenticated GET.\napi: SynSense Website Content API\nbase_url: https://www.synsense.ai/wp-json\nanonymous_read: true\nanonymous_read_evidence: >-\n  GET /wp/v2/products_list, /careers_list, /our_partners, /awards, /office, /posts, /pages,\n  /media, /categories, /tags, /types, /taxonomies, /statuses, /search and /users each returned\n  HTTP 200 with a JSON array and an X-WP-Total header, with no credentials of any kind.\nschemes:\n- id: none\n  type: none\n  applies_to: >-\n    All GET operations in openapi/aictx-website-content-api-openapi.json\
  \ (40 of 40). The derived\n    document sets `security: []` on every operation to state this explicitly.\n  note: >-\n    WordPress serves the `view` context of public post types to anonymous callers. The `edit`\n    context is refused with 401 rest_forbidden_context.\n- id: application-passwords\n  type: http\n  scheme: basic\n  applies_to: >-\n    The write surface (POST/PUT/PATCH/DELETE) and any `context=edit` read. Not described in the\n    derived OpenAPI, because it was never exercised and no SynSense documentation covers it.\n  authorization_endpoint: https://www.synsense.ai/wp-admin/authorize-application.php\n  source: >-\n    The `authentication` object in the live route index:\n    {\"application-passwords\":{\"endpoints\":{\"authorization\":\"https://www.synsense.ai/wp-admin/authorize-application.php\"}}}\n  note: >-\n    WordPress application passwords are sent as HTTP Basic (username + generated password). This\n    is site-administrator credentialing, not a developer program\
  \ — SynSense issues no API keys and\n    publishes no onboarding path for it.\n- id: cookie-nonce\n  type: apiKey\n  in: header\n  name: X-WP-Nonce\n  applies_to: Browser sessions inside the site's own admin/editor.\n  source: >-\n    Advertised by the live response header\n    `access-control-allow-headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type`.\nobserved_refusals:\n- request: GET /wp/v2/products_list?context=edit\n  status: 401\n  code: rest_forbidden_context\n- request: GET /wp/v2/users/me\n  status: 401\n  code: rest_not_logged_in\n- request: GET /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- request: POST /wp/v2/comments\n  status: 401\n  code: rest_comment_login_required\ncors:\n  access_control_allow_origin: '*'\n  access_control_allow_methods: GET, POST, OPTIONS\n  access_control_expose_headers: X-WP-Total, X-WP-TotalPages, Link\n  note: >-\n    Origin `*` on a read-only public content surface. Browser-callable from anywhere without\
  \ a\n    proxy.\noauth: false\noauth_note: >-\n  No OAuth 2.0 or OpenID Connect surface exists. /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both 404 on every host (see well-known/). No scopes/\n  artifact is written for this provider for that reason.\ndeveloper_program:\n  api_keys_issued: false\n  signup_url: https://www.synsense.ai/login/\n  signup_note: >-\n    The synsense.ai login is for the developer community forum and the gated download centre,\n    not for API credentials. SynSense issues no API keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/authentication/aictx-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Neuromorphic Computing
- Artificial Intelligence
- Semiconductors
- Edge Computing
- Machine Learning
- Sensors
- IoT
- Open Source
---
