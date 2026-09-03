---
api_key_in: []
api_specs:
- filename: perfect-corp-ai_abs_filter-openapi.yml
  format: yaml
  label: YouCam AI REST API
  slug: youcam-ai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perfect-corp/refs/heads/main/openapi/perfect-corp-ai_abs_filter-openapi.yml
auth_types:
- http
description: 'One credential covers the whole platform: a YouCam API key sent as an HTTP bearer token. The same key authenticates the REST API and all three hosted MCP servers. An OAuth 2.0 authorization server is ALSO discoverable at the API host well-known path, but nothing in the developer documentation references it and no published operation requires it.'
kind: authentication
layout: security
method: searched
name: Perfect Corp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perfect Corp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perfect Corp
provider_slug: perfect-corp
scheme_count: 1
schemes:
- description: 'Use the standard ''Bearer authentication''. Put your ''API Key'' in header: `Authorization:Bearer YOUR_API_KEY`. Notice that there is '' '' a space between ''Bearer'' and the ''YOUR_API_KEY''.'
  name: BearerAuthenticationV2
  scheme: bearer
  sources:
  - openapi/perfect-corp-ai_abs_filter-openapi.yml
  - openapi/perfect-corp-ai_aging_simulation-openapi.yml
  - openapi/perfect-corp-ai_avatar_generator-openapi.yml
  - openapi/perfect-corp-ai_background_removal-openapi.yml
  - openapi/perfect-corp-ai_bag-openapi.yml
  - openapi/perfect-corp-ai_bangs-openapi.yml
  - openapi/perfect-corp-ai_beard_style-openapi.yml
  - openapi/perfect-corp-ai_body_reshape-openapi.yml
  - openapi/perfect-corp-ai_bracelet-openapi.yml
  - openapi/perfect-corp-ai_breast_augmentation-openapi.yml
  - openapi/perfect-corp-ai_clothes-openapi.yml
  - openapi/perfect-corp-ai_color_correction-openapi.yml
  - openapi/perfect-corp-ai_earrings-openapi.yml
  - openapi/perfect-corp-ai_eye_color_lens-openapi.yml
  - openapi/perfect-corp-ai_fabric-openapi.yml
  - openapi/perfect-corp-ai_face_analyzer-openapi.yml
  - openapi/perfect-corp-ai_face_lift-openapi.yml
  - openapi/perfect-corp-ai_face_reshape-openapi.yml
  - openapi/perfect-corp-ai_face_swap-openapi.yml
  - openapi/perfect-corp-ai_fitzpatrick_skin_type-openapi.yml
  - openapi/perfect-corp-ai_hair_color-openapi.yml
  - openapi/perfect-corp-ai_hair_density_detection-openapi.yml
  - openapi/perfect-corp-ai_hair_extension-openapi.yml
  - openapi/perfect-corp-ai_hair_frizziness_detection-openapi.yml
  - openapi/perfect-corp-ai_hair_length_detection-openapi.yml
  - openapi/perfect-corp-ai_hair_type_detection-openapi.yml
  - openapi/perfect-corp-ai_hair_volume-openapi.yml
  - openapi/perfect-corp-ai_hairstyle-openapi.yml
  - openapi/perfect-corp-ai_hat-openapi.yml
  - openapi/perfect-corp-ai_headshot_generator-openapi.yml
  - openapi/perfect-corp-ai_image_extender-openapi.yml
  - openapi/perfect-corp-ai_image_generator-openapi.yml
  - openapi/perfect-corp-ai_look_vto-openapi.yml
  - openapi/perfect-corp-ai_makeup_transfer-openapi.yml
  - openapi/perfect-corp-ai_nail_transfer-openapi.yml
  - openapi/perfect-corp-ai_nail_vto-openapi.yml
  - openapi/perfect-corp-ai_necklace-openapi.yml
  - openapi/perfect-corp-ai_object_removal_pro-openapi.yml
  - openapi/perfect-corp-ai_photo_background_blur-openapi.yml
  - openapi/perfect-corp-ai_photo_background_change-openapi.yml
  - openapi/perfect-corp-ai_photo_colorize-openapi.yml
  - openapi/perfect-corp-ai_photo_enhance-openapi.yml
  - openapi/perfect-corp-ai_photo_lighting-openapi.yml
  - openapi/perfect-corp-ai_replace-openapi.yml
  - openapi/perfect-corp-ai_scarf-openapi.yml
  - openapi/perfect-corp-ai_shoes-openapi.yml
  - openapi/perfect-corp-ai_skin_analysis-openapi.yml
  - openapi/perfect-corp-ai_skin_simulation-openapi.yml
  - openapi/perfect-corp-ai_skin_tone_analysis-openapi.yml
  - openapi/perfect-corp-ai_smile-openapi.yml
  - openapi/perfect-corp-ai_studio_generator-openapi.yml
  - openapi/perfect-corp-ai_teeth_whitening-openapi.yml
  - openapi/perfect-corp-ai_video_background_replace-openapi.yml
  - openapi/perfect-corp-ai_video_enhancer-openapi.yml
  - openapi/perfect-corp-ai_video_face_swap-openapi.yml
  - openapi/perfect-corp-ai_video_generator-openapi.yml
  - openapi/perfect-corp-ai_video_object_removal-openapi.yml
  - openapi/perfect-corp-ai_video_style_transfer-openapi.yml
  - openapi/perfect-corp-ai_watch-openapi.yml
  - openapi/perfect-corp-ai_wavy_hair-openapi.yml
  - openapi/perfect-corp-file-openapi.yml
  - openapi/perfect-corp-makeup_vto-openapi.yml
  - openapi/perfect-corp-ring_vto-openapi.yml
  - openapi/perfect-corp-task_management-openapi.yml
  - openapi/perfect-corp-unit_system-openapi.yml
  type: http
slug: perfect-corp-authentication
source_filename: perfect-corp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://docs.perfectcorp.com/develop/quick_start_guide, /develop/debugging_guide, /develop/mcp, https://yce-api-01.makeupar.com/.well-known/oauth-authorization-server,\n  and the 65 published OpenAPI 3.0.0 documents in openapi/.\ndocs: https://docs.perfectcorp.com/develop/quick_start_guide\nname: Perfect Corp YouCam API — authentication\ndescription: 'One credential covers the whole platform: a YouCam API key sent as an HTTP bearer token. The same\n  key authenticates the REST API and all three hosted MCP servers. An OAuth 2.0 authorization server is ALSO discoverable\n  at the API host well-known path, but nothing in the developer documentation references it and no published operation\n  requires it.'\nprimary:\n  scheme: http-bearer\n  header: 'Authorization: Bearer <YOUR_API_KEY>'\n  applies_to:\n  - REST API (all 178 published operations)\n  - MCP servers beauty / fashion / creators\n  key_management: https://yce.perfectcorp.com/api-console/en/api-keys/\n\
  \  signup: https://yce.perfectcorp.com/ai-api\n  key_prefix: null\n  rotation: Keys are generated and maintained in the API Console; no rotation policy or expiry period is published.\n  documented_failure_modes:\n  - 'Missing the \"Bearer \" prefix — send `Authorization: Bearer KEY`, not `Authorization: KEY`.'\n  - Wrapping the key in angle brackets (`Bearer <KEY>`) — the brackets are sent literally and the request fails.\n  - Inactive or expired key — error codes InactiveApiKey / ExpiredApiKey.\n  error_codes:\n  - InvalidApiKey\n  - InactiveApiKey\n  - ExpiredApiKey\nlegacy:\n  scheme: http-bearer (exchanged access_token)\n  name: BearerAuthentication\n  flow: POST /s2s/v1.0/client/auth exchanges client credentials for a short-lived access_token.\n  status: still declared in the contracts alongside the V2 scheme; no end-of-life date is published.\n  error_code: InvalidAccessToken\n  note: Only the unit_system contract still applies this scheme to an operation; every AI feature uses BearerAuthenticationV2.\n\
  oauth2:\n  discoverable: true\n  metadata_url: https://yce-api-01.makeupar.com/.well-known/oauth-authorization-server\n  issuer: https://yce-api-01.perfectcorp.com\n  documented_in_developer_docs: false\n  referenced_by_any_operation: false\n  detail: scopes/perfect-corp-scopes.yml\n  note: An RFC 8414 authorization-server metadata document is served anonymously and describes a public-client authorization_code\n    + PKCE S256 flow with dynamic client registration and two scopes (task.run, task.read). It appears nowhere in\n    the API reference, the quick start, or the MCP page — an undocumented but real second authentication surface.\nmtls: false\nopenid_connect: false\napi_key_in_query: false\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuthenticationV2\n  type: http\n  scheme: bearer\n  description: 'Use the standard ''Bearer authentication''. Put your ''API Key'' in header: `Authorization:Bearer\n    YOUR_API_KEY`. Notice that there is '' '' a space between ''Bearer'' and\
  \ the ''YOUR_API_KEY''.'\n  sources:\n  - openapi/perfect-corp-ai_abs_filter-openapi.yml\n  - openapi/perfect-corp-ai_aging_simulation-openapi.yml\n  - openapi/perfect-corp-ai_avatar_generator-openapi.yml\n  - openapi/perfect-corp-ai_background_removal-openapi.yml\n  - openapi/perfect-corp-ai_bag-openapi.yml\n  - openapi/perfect-corp-ai_bangs-openapi.yml\n  - openapi/perfect-corp-ai_beard_style-openapi.yml\n  - openapi/perfect-corp-ai_body_reshape-openapi.yml\n  - openapi/perfect-corp-ai_bracelet-openapi.yml\n  - openapi/perfect-corp-ai_breast_augmentation-openapi.yml\n  - openapi/perfect-corp-ai_clothes-openapi.yml\n  - openapi/perfect-corp-ai_color_correction-openapi.yml\n  - openapi/perfect-corp-ai_earrings-openapi.yml\n  - openapi/perfect-corp-ai_eye_color_lens-openapi.yml\n  - openapi/perfect-corp-ai_fabric-openapi.yml\n  - openapi/perfect-corp-ai_face_analyzer-openapi.yml\n  - openapi/perfect-corp-ai_face_lift-openapi.yml\n  - openapi/perfect-corp-ai_face_reshape-openapi.yml\n  -\
  \ openapi/perfect-corp-ai_face_swap-openapi.yml\n  - openapi/perfect-corp-ai_fitzpatrick_skin_type-openapi.yml\n  - openapi/perfect-corp-ai_hair_color-openapi.yml\n  - openapi/perfect-corp-ai_hair_density_detection-openapi.yml\n  - openapi/perfect-corp-ai_hair_extension-openapi.yml\n  - openapi/perfect-corp-ai_hair_frizziness_detection-openapi.yml\n  - openapi/perfect-corp-ai_hair_length_detection-openapi.yml\n  - openapi/perfect-corp-ai_hair_type_detection-openapi.yml\n  - openapi/perfect-corp-ai_hair_volume-openapi.yml\n  - openapi/perfect-corp-ai_hairstyle-openapi.yml\n  - openapi/perfect-corp-ai_hat-openapi.yml\n  - openapi/perfect-corp-ai_headshot_generator-openapi.yml\n  - openapi/perfect-corp-ai_image_extender-openapi.yml\n  - openapi/perfect-corp-ai_image_generator-openapi.yml\n  - openapi/perfect-corp-ai_look_vto-openapi.yml\n  - openapi/perfect-corp-ai_makeup_transfer-openapi.yml\n  - openapi/perfect-corp-ai_nail_transfer-openapi.yml\n  - openapi/perfect-corp-ai_nail_vto-openapi.yml\n\
  \  - openapi/perfect-corp-ai_necklace-openapi.yml\n  - openapi/perfect-corp-ai_object_removal_pro-openapi.yml\n  - openapi/perfect-corp-ai_photo_background_blur-openapi.yml\n  - openapi/perfect-corp-ai_photo_background_change-openapi.yml\n  - openapi/perfect-corp-ai_photo_colorize-openapi.yml\n  - openapi/perfect-corp-ai_photo_enhance-openapi.yml\n  - openapi/perfect-corp-ai_photo_lighting-openapi.yml\n  - openapi/perfect-corp-ai_replace-openapi.yml\n  - openapi/perfect-corp-ai_scarf-openapi.yml\n  - openapi/perfect-corp-ai_shoes-openapi.yml\n  - openapi/perfect-corp-ai_skin_analysis-openapi.yml\n  - openapi/perfect-corp-ai_skin_simulation-openapi.yml\n  - openapi/perfect-corp-ai_skin_tone_analysis-openapi.yml\n  - openapi/perfect-corp-ai_smile-openapi.yml\n  - openapi/perfect-corp-ai_studio_generator-openapi.yml\n  - openapi/perfect-corp-ai_teeth_whitening-openapi.yml\n  - openapi/perfect-corp-ai_video_background_replace-openapi.yml\n  - openapi/perfect-corp-ai_video_enhancer-openapi.yml\n\
  \  - openapi/perfect-corp-ai_video_face_swap-openapi.yml\n  - openapi/perfect-corp-ai_video_generator-openapi.yml\n  - openapi/perfect-corp-ai_video_object_removal-openapi.yml\n  - openapi/perfect-corp-ai_video_style_transfer-openapi.yml\n  - openapi/perfect-corp-ai_watch-openapi.yml\n  - openapi/perfect-corp-ai_wavy_hair-openapi.yml\n  - openapi/perfect-corp-file-openapi.yml\n  - openapi/perfect-corp-makeup_vto-openapi.yml\n  - openapi/perfect-corp-ring_vto-openapi.yml\n  - openapi/perfect-corp-task_management-openapi.yml\n  - openapi/perfect-corp-unit_system-openapi.yml\nx-evidence:\n- url: https://docs.perfectcorp.com/develop/quick_start_guide\n  http_status: 200\n- url: https://docs.perfectcorp.com/develop/debugging_guide.md\n  http_status: 200\n- url: https://yce-api-01.makeupar.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://yce-api-01.makeupar.com/s2s/v2.0/credit/feature-cost\n  http_status: 401\n  body: '{\"status\":401,\"error\":\"This API key is\
  \ not recognized.\",\"error_code\":\"InvalidApiKey\"}'\n- url: https://yce.perfectcorp.com/api-console/en/api-keys/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfect-corp/refs/heads/main/authentication/perfect-corp-authentication.yml
summary_line: http · 1 scheme
tags:
- beauty
- skincare
- cosmetics
- fashion
- apparel
- jewelry
- watches
- hair
- virtual-try-on
- image-editing
- generative-ai
- computer-vision
- AR
- visual-commerce
- ai
- machine-learning
- video-generation
- skin-analysis
- mcp
- agents
- photo-editing
- beauty-tech
- retail
- ar-try-on
---
