---
api_key_in: []
auth_types: []
description: Fashion Diffusion authenticates every Public API call with a single long-lived bearer API key. There is no OAuth 2.0 authorization server, no OpenID Connect discovery document, no mutual TLS and no scope surface — a key is either valid or it is not, and its authority is bounded by the user and team that own it.
kind: authentication
layout: security
method: searched
name: Fashiondiffusion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fashion Diffusion declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fashion Diffusion
provider_slug: fashiondiffusion
scheme_count: 1
schemes:
- applies_to: all documented Public API operations
  description: '"Create an API key and send the complete secret as a bearer credential. The secret is displayed only once." (docs, Authentication section)'
  evidence:
    status: 200
    url: https://www.fashiondiffusion.ai/playground/api/docs
  format: 'Authorization: Bearer fd_live_xxx'
  header: Authorization
  id: bearerApiKey
  in: header
  key_prefix: fd_live_
  scheme: bearer
  type: http
slug: fashiondiffusion-authentication
source_filename: fashiondiffusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: searched\nsource: https://www.fashiondiffusion.ai/playground/api/docs\nname: Fashion Diffusion Public API — Authentication\ndescription: >-\n  Fashion Diffusion authenticates every Public API call with a single long-lived\n  bearer API key. There is no OAuth 2.0 authorization server, no OpenID Connect\n  discovery document, no mutual TLS and no scope surface — a key is either valid\n  or it is not, and its authority is bounded by the user and team that own it.\ndocs: https://www.fashiondiffusion.ai/playground/api/docs\nkey_management_url: https://www.fashiondiffusion.ai/playground/api\nschemes:\n  - id: bearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer fd_live_xxx'\n    key_prefix: fd_live_\n    description: >-\n      \"Create an API key and send the complete secret as a bearer credential.\n      The secret is displayed only once.\" (docs, Authentication section)\n\
  \    applies_to: all documented Public API operations\n    evidence:\n      url: https://www.fashiondiffusion.ai/playground/api/docs\n      status: 200\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  present: false\n  note: >-\n    No scope, permission or role surface is documented. Authority is implicit:\n    \"An API key can only read tasks owned by its user and current team.\"\nkey_lifecycle:\n  created_at: https://www.fashiondiffusion.ai/playground/api\n  secret_display: once-only at creation\n  rotation_documented: false\n  expiry_documented: false\n  revocation_documented: false\n  multiple_keys_per_user: true\n  note: >-\n    Docs state task listing includes \"tasks submitted with any of the user's API\n    keys\", which confirms a user may hold more than one key. Rotation, expiry and\n    revocation procedures are not documented publicly.\nfailure_mode:\n  status: 401\n  body: '{\"error\":{\"code\":\"INVALID_API_KEY\",\"message\":\"Invalid API key\",\"requestId\"\
  :\"<uuid>\"}}'\n  method: probed\n  evidence:\n    - url: https://www.fashiondiffusion.ai/api/public/v1/tasks\n      status: 401\n      note: unauthenticated GET, observed 2026-08-31\n    - url: https://www.fashiondiffusion.ai/api/public/v1/virtual-try-on/tasks\n      status: 401\n      note: unauthenticated POST with empty JSON body, observed 2026-08-31\ngaps:\n  - No machine-readable contract declares this scheme; it exists only as prose plus\n    curl examples on the docs page.\n  - No documented key rotation or revocation path.\n  - Access to a key requires a paid plan sign-in; the docs page itself is anonymous.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fashiondiffusion/refs/heads/main/authentication/fashiondiffusion-authentication.yml
summary_line: 1 scheme
tags:
- Fashion
- E-Commerce
- Retail
- Generative AI
- Image-Generation
- Virtual Try-On
- Computer-Vision
- Video Generation
- Product Photography
- Creative / Design Tools
---
