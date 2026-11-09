---
anonymous_access: false
api_key_in: []
api_specs:
- filename: transcriptapi-com-youtube-channel-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube channel API
  slug: transcriptapi-com-youtube-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-channel-api-openapi.yml
- filename: transcriptapi-com-youtube-playlist-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube playlist API
  slug: transcriptapi-com-youtube-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-playlist-api-openapi.yml
- filename: transcriptapi-com-youtube-search-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube search API
  slug: transcriptapi-com-youtube-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-search-api-openapi.yml
- filename: transcriptapi-com-youtube-transcript-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube transcript API
  slug: transcriptapi-com-youtube-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-transcript-api-openapi.yml
- filename: transcriptapi-com-youtube-video-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube video API
  slug: transcriptapi-com-youtube-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-video-api-openapi.yml
auth_types: []
description: Authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Transcriptapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: transcriptapi-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: transcriptapi-com
provider_slug: transcriptapi-com
scheme_count: 1
schemes:
- evidence: 'The shortest version, once you have an API key :

    Terminal window curl -G " https://transcriptapi.com/api/v2/youtube/transcript " \ --data-urlencode " video_url=https://www.youtube.com/watch?v=dQw4w9WgXcQ " \ -H " Authorization: Bearer YOUR_API_KEY "'
  header: Authorization
  how_to_obtain: Sign up for an API key on the TranscriptAPI website and copy it from the API Keys dashboard.
  location: header
  name: Authorization
  type: apiKey
slug: transcriptapi-com-authentication
source_filename: transcriptapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://transcriptapi.com/docs/getting-started/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://transcriptapi.com/docs/getting-started/\nsources:\n- https://transcriptapi.com/docs/getting-started/\n- https://transcriptapi.com/docs/getting-started/python/\n- https://transcriptapi.com/docs/getting-started/javascript/\n- https://transcriptapi.com/docs/getting-started/curl/\ndescription: Authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'The shortest version, once you have an API key :\n\n    Terminal window curl -G \" https://transcriptapi.com/api/v2/youtube/transcript \" \\ --data-urlencode \" video_url=https://www.youtube.com/watch?v=dQw4w9WgXcQ\n    \" \\ -H \" Authorization: Bearer YOUR_API_KEY \"'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up for an API key on the TranscriptAPI website and copy it from the API Keys dashboard.\nnote: No OAuth2 or\
  \ other authentication methods are documented on the provided pages.\ndocs: https://transcriptapi.com/docs/getting-started/\n"
source_yaml_url: https://artifacts.apis.io/transcriptapi-com/authentication/transcriptapi-com-authentication.yml
summary_line: 1 scheme
tags:
- Transcripts
- YouTube API
- Search
- Content Extraction
---
