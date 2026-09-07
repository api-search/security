---
anonymous_access: false
api_key_in: []
api_specs:
- filename: magichour-audio-projects-api-openapi.yml
  format: yaml
  label: Magic Hour Audio Projects API
  slug: magichour-audio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-audio-projects-api-openapi.yml
- filename: magichour-files-api-openapi.yml
  format: yaml
  label: Magic Hour Files API
  slug: magichour-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-files-api-openapi.yml
- filename: magichour-image-projects-api-openapi.yml
  format: yaml
  label: Magic Hour Image Projects API
  slug: magichour-image-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-image-projects-api-openapi.yml
- filename: magichour-video-projects-api-openapi.yml
  format: yaml
  label: Magic Hour Video Projects API
  slug: magichour-video-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/openapi/magichour-video-projects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Magichour Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magic Hour secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Magic Hour
provider_slug: magichour
scheme_count: 1
schemes:
- description: Bearer authentication header of the form `Bearer <api_key>`, where `<api_key>` is your API key. To get your API key, go to [Developer Hub](https://magichour.ai/developer?tab=api-keys&utm_source=docs&utm_medium=referral&utm_campaign=api-reference) and click "Create new API Key".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/magichour-audio-projects-api-openapi.yml
  - openapi/magichour-files-api-openapi.yml
  - openapi/magichour-image-projects-api-openapi.yml
  - openapi/magichour-video-projects-api-openapi.yml
  type: http
slug: magichour-authentication
source_filename: magichour-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/magichour-audio-projects-api-openapi.yml, openapi/magichour-files-api-openapi.yml,\n  openapi/magichour-image-projects-api-openapi.yml, openapi/magichour-video-projects-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication header of the form `Bearer <api_key>`, where `<api_key>`\n    is your API key. To get your API key, go to [Developer Hub](https://magichour.ai/developer?tab=api-keys&utm_source=docs&utm_medium=referral&utm_campaign=api-reference)\n    and click \"Create new API Key\".\n  sources:\n  - openapi/magichour-audio-projects-api-openapi.yml\n  - openapi/magichour-files-api-openapi.yml\n  - openapi/magichour-image-projects-api-openapi.yml\n  - openapi/magichour-video-projects-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magichour/refs/heads/main/authentication/magichour-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Video
- Image-Generation
- Audio
- Generative AI
- Voice Cloning
- Text-To-Video
---
