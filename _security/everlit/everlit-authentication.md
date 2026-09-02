---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Everlit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everlit declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Everlit
provider_slug: everlit
scheme_count: 4
schemes:
- applies_to:
  - GET https://everlit.audio/oembed?url=<embed-or-hosted-url>
  - GET https://everlit.audio/embeds/{track_id}.json
  - GET https://everlit.audio/embeds/{id}
  - GET https://everlit.audio/hosted/{artl_id}
  description: 'The oEmbed resolver and the player bootstrap JSON answer anonymously. Verified 2026-08-20: HTTP 200 with no credential of any kind.'
  evidence:
    http_status: 200
    url: https://everlit.audio/oembed?url=https%3A%2F%2Feverlit.audio%2Fembeds%2Fartl_9QemEuv4WkQ
  id: none-public-embed
  type: none
- applies_to:
  - Everlit REST API (undocumented, access-gated)
  - Everlit WordPress plugin configuration
  description: Everlit's own WordPress dispatch states that plugin "configuration requires only your Everlit API key". The key is issued through onboarding; Everlit publishes no key format, no header name, no rotation policy, no scope model and no self-serve key-issuance page.
  evidence:
    http_status: 200
    url: https://everlit.audio/dispatches/wordpress-plugin-audio-articles-newspack
  gaps:
  - Header/parameter name not published.
  - No key prefix or format documented.
  - No rotation, expiry or revocation policy published.
  - No self-serve issuance — keys come from sales/onboarding via hello@everlit.audio.
  id: api-key
  in: unknown
  name: unknown
  type: apiKey
- applies_to:
  - https://studio.everlit.audio (Everlit Studio web console)
  description: The Studio is a Rails application; the root 302s to /session/new and the HTML carries a csrf-token meta. Browser session auth only — not an agent-callable surface.
  evidence:
    http_status: 200
    redirects_to: https://studio.everlit.audio/session/new
    url: https://studio.everlit.audio/
  id: session-cookie
  scheme: session
  type: http
- applies_to:
  - GET https://everlit.audio/embeds/{track_id}/playlist?ste=<token>
  - Player analytics/share/capture callbacks
  description: The player bootstrap JSON hands the client a base64 `ste` stream token and a signed `auth_key` (a Rails message-verifier blob of the shape "<base64 payload>--<hmac>") that carries a user_tag, session_tag, article_id, channel and ad_context. These are short-lived, issued per playback, and are not credentials a developer can obtain or manage.
  evidence:
    http_status: 200
    note: A request to /embeds/{id}/playlist without a live token returns HTTP 400, confirming the token is enforced rather than decorative.
    url: https://everlit.audio/embeds/artl_9QemEuv4WkQ.json
  id: signed-playback-token
  type: signed-token
slug: everlit-authentication
source_filename: everlit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: searched\nsource: >-\n  https://everlit.audio/dispatches/wordpress-plugin-audio-articles-newspack (API key statement),\n  https://everlit.audio/llms-full.txt, plus live probes of https://everlit.audio/oembed,\n  https://everlit.audio/embeds/<id>.json and https://studio.everlit.audio — 2026-08-20.\ndocs: null\nsummary: >-\n  Everlit publishes no authentication reference page and no securitySchemes (there is no OpenAPI).\n  Three distinct auth postures were established from the vendor's own copy and from live probes.\n  Nothing here is inferred from a spec: every entry names the URL it came from.\n\nschemes:\n- id: none-public-embed\n  type: none\n  applies_to:\n  - GET https://everlit.audio/oembed?url=<embed-or-hosted-url>\n  - GET https://everlit.audio/embeds/{track_id}.json\n  - GET https://everlit.audio/embeds/{id}\n  - GET https://everlit.audio/hosted/{artl_id}\n  description: >-\n    The oEmbed resolver and the player bootstrap JSON answer\
  \ anonymously. Verified 2026-08-20:\n    HTTP 200 with no credential of any kind.\n  evidence:\n    url: https://everlit.audio/oembed?url=https%3A%2F%2Feverlit.audio%2Fembeds%2Fartl_9QemEuv4WkQ\n    http_status: 200\n\n- id: api-key\n  type: apiKey\n  applies_to:\n  - Everlit REST API (undocumented, access-gated)\n  - Everlit WordPress plugin configuration\n  in: unknown\n  name: unknown\n  description: >-\n    Everlit's own WordPress dispatch states that plugin \"configuration requires only your Everlit\n    API key\". The key is issued through onboarding; Everlit publishes no key format, no header\n    name, no rotation policy, no scope model and no self-serve key-issuance page.\n  evidence:\n    url: https://everlit.audio/dispatches/wordpress-plugin-audio-articles-newspack\n    http_status: 200\n  gaps:\n  - Header/parameter name not published.\n  - No key prefix or format documented.\n  - No rotation, expiry or revocation policy published.\n  - No self-serve issuance — keys come from\
  \ sales/onboarding via hello@everlit.audio.\n\n- id: session-cookie\n  type: http\n  scheme: session\n  applies_to:\n  - https://studio.everlit.audio (Everlit Studio web console)\n  description: >-\n    The Studio is a Rails application; the root 302s to /session/new and the HTML carries a\n    csrf-token meta. Browser session auth only — not an agent-callable surface.\n  evidence:\n    url: https://studio.everlit.audio/\n    http_status: 200\n    redirects_to: https://studio.everlit.audio/session/new\n\n- id: signed-playback-token\n  type: signed-token\n  applies_to:\n  - GET https://everlit.audio/embeds/{track_id}/playlist?ste=<token>\n  - Player analytics/share/capture callbacks\n  description: >-\n    The player bootstrap JSON hands the client a base64 `ste` stream token and a signed `auth_key`\n    (a Rails message-verifier blob of the shape \"<base64 payload>--<hmac>\") that carries a user_tag,\n    session_tag, article_id, channel and ad_context. These are short-lived, issued per\
  \ playback,\n    and are not credentials a developer can obtain or manage.\n  evidence:\n    url: https://everlit.audio/embeds/artl_9QemEuv4WkQ.json\n    http_status: 200\n    note: >-\n      A request to /embeds/{id}/playlist without a live token returns HTTP 400, confirming the\n      token is enforced rather than decorative.\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\nmfa_documented: false\n\nfindings:\n- The only agent-reachable Everlit surface needs no credential at all; the only credentialed\n  surface (the REST API) has no public documentation, so an agent cannot self-onboard.\n- No /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource or\n  /.well-known/openid-configuration on any Everlit host (all 404, 2026-08-20).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlit/refs/heads/main/authentication/everlit-authentication.yml
summary_line: 4 schemes
tags:
- Audio
- Video
- Social
- Podcasts
- Media
- Publishers
- News
- Text-to-Speech
- AI-voice
- Content Distribution
- Monetization
- Accessibility
- oEmbed
- embeddable-player
- Advertising
---
