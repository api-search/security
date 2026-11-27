---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meetstream-ai-bots-api-openapi.yml
  format: yaml
  label: MeetStream.ai Bots API
  slug: meetstream-ai-bots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetstream-ai/openapi/meetstream-ai-bots-api-openapi.yml
- filename: meetstream-ai-calendar-api-openapi.yml
  format: yaml
  label: MeetStream.ai Calendar API
  slug: meetstream-ai-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetstream-ai/openapi/meetstream-ai-calendar-api-openapi.yml
- filename: meetstream-ai-googlelogin-api-openapi.yml
  format: yaml
  label: MeetStream.ai Google Login API
  slug: meetstream-ai-googlelogin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetstream-ai/openapi/meetstream-ai-googlelogin-api-openapi.yml
- filename: meetstream-ai-mia-api-openapi.yml
  format: yaml
  label: MeetStream.ai Mia API
  slug: meetstream-ai-mia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetstream-ai/openapi/meetstream-ai-mia-api-openapi.yml
- filename: meetstream-ai-teamslogin-api-openapi.yml
  format: yaml
  label: MeetStream.ai Teams Login API
  slug: meetstream-ai-teamslogin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetstream-ai/openapi/meetstream-ai-teamslogin-api-openapi.yml
- filename: meetstream-ai-transcription-api-openapi.yml
  format: yaml
  label: MeetStream.ai Transcription API
  slug: meetstream-ai-transcription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetstream-ai/openapi/meetstream-ai-transcription-api-openapi.yml
auth_types: []
description: All MeetStream API requests require an API key. Send it in the `Authorization` header of every request, prefixed with `Token`.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MeetStream.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: MeetStream.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MeetStream.ai
provider_slug: meetstream-ai
scheme_count: 1
schemes:
- evidence: All MeetStream API requests require an API key. Send it in the `Authorization` header of every request, prefixed with `Token`.
  header: Authorization
  how_to_obtain: Create an API key in the MeetStream dashboard under the API Keys section.
  location: header
  name: Token
  type: other
slug: meetstream-ai-authentication
source_filename: meetstream-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.meetstream.ai/guides/app-integrations/zoom-oauth-meeting-bots.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.meetstream.ai/guides/app-integrations/zoom-oauth-meeting-bots.md\nsources:\n- https://docs.meetstream.ai/guides/app-integrations/zoom-oauth-meeting-bots.md\n- https://docs.meetstream.ai/guides/calendar-integrations/google-calendar-oauth-setup.md\n- https://docs.meetstream.ai/api-reference/authentication.md\n- https://docs.meetstream.ai/guides/get-started/dashboard-setup.md\ndescription: All MeetStream API requests require an API key. Send it in the `Authorization` header of every request, prefixed with `Token`.\nschemes:\n- type: other\n  name: Token\n  evidence: All MeetStream API requests require an API key. Send it in the `Authorization` header of every request, prefixed with `Token`.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the MeetStream dashboard under the API Keys section.\ndocs: https://docs.meetstream.ai/guides/app-integrations/zoom-oauth-meeting-bots.md\n"
source_yaml_url: https://artifacts.apis.io/meetstream-ai/authentication/meetstream-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Meetings
- Video
- Audio
- Automation
---
