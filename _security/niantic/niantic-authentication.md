---
api_key_in:
- sdk-config
auth_types:
- apiKey
- token
description: ''
kind: authentication
layout: security
method: searched
name: Niantic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Niantic secures its APIs with apiKey and token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Niantic
provider_slug: niantic
scheme_count: 2
schemes:
- description: NSDK 4.0 introduced a token-based authentication model for the Niantic Spatial platform, replacing the legacy API-key-only approach. Simplifies auth for testing and iteration across Unity, Swift, and Kotlin.
  name: NianticSpatialToken
  scheme: bearer-token
  since: NSDK 4.0
  sources:
  - docs
  type: token
- deprecated: true
  description: Legacy Lightship ARDK model. An API key created in the developer account is configured into the app; VPS validates the app's API key against the developer account. Superseded by token-based auth in NSDK 4.0.
  in: sdk-config
  name: LightshipApiKey
  sources:
  - docs
  type: apiKey
slug: niantic-authentication
source_filename: niantic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.nianticspatial.com/docs/nsdk/\ndocs: https://www.nianticspatial.com/docs/nsdk/\nnotes: >-\n  No OpenAPI is published for the Niantic Spatial platform (SDK-first: Unity/Swift/\n  Kotlin/ROS 2), so this profile is captured from the developer documentation rather\n  than derived from a spec. Two documented models coexist across SDK generations.\nsummary:\n  types: [apiKey, token]\n  api_key_in: [sdk-config]\nschemes:\n  - name: NianticSpatialToken\n    type: token\n    scheme: bearer-token\n    description: >-\n      NSDK 4.0 introduced a token-based authentication model for the Niantic\n      Spatial platform, replacing the legacy API-key-only approach. Simplifies\n      auth for testing and iteration across Unity, Swift, and Kotlin.\n    since: NSDK 4.0\n    sources: [docs]\n  - name: LightshipApiKey\n    type: apiKey\n    in: sdk-config\n    description: >-\n      Legacy Lightship ARDK model. An API key created\
  \ in the developer account is\n      configured into the app; VPS validates the app's API key against the\n      developer account. Superseded by token-based auth in NSDK 4.0.\n    deprecated: true\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niantic/refs/heads/main/authentication/niantic-authentication.yml
summary_line: apiKey/token · 2 schemes
tags:
- Company
- Geospatial
- Augmented Reality
- Computer Vision
- Visual Positioning
- Spatial Computing
- SDK
- Physical AI
- Robotics
---
