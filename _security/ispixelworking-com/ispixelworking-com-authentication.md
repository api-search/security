---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ispixelworking-com-openapi-generated.yml
  format: yaml
  label: IsPixelWorking API
  slug: ispixelworking-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ispixelworking-com/openapi/_ae-authored/ispixelworking-com-openapi-generated.yml
auth_types: []
description: Authentication methods for OpenAI Conversions API and TikTok Events API as described on IsPixelWorking pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: IsPixelWorking Authentication
name_suffix: Authentication
oauth_flows: []
overview: IsPixelWorking declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: IsPixelWorking
provider_slug: ispixelworking-com
scheme_count: 2
schemes:
- evidence: 'Send a POST request to https://bzr.openai.com/v1/events?pid=<PIXEL-ID> with your Conversions API key as a bearer token:'
  header: Authorization
  how_to_obtain: Provision it from the conversions tab in Ads Manager, or create it with your Advertiser API key (POST /v1/conversions/api_keys).
  location: header
  name: OpenAI Conversions API key
  type: http-bearer
- evidence: 'Send events in a POST request to https://business-api.tiktok.com/open_api/v1.3/event/track/ with the headers Access-Token: <your token> and Content-Type: application/json .'
  header: Access-Token
  how_to_obtain: Generate an access token in Events Manager under the pixel Settings tab by clicking Generate Access Token.
  location: header
  name: TikTok Access Token
  type: http-bearer
slug: ispixelworking-com-authentication
source_filename: ispixelworking-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ispixelworking.com/guides/openai.conversions_api_setup/generic
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ispixelworking.com/guides/openai.conversions_api_setup/generic\nsources:\n- https://ispixelworking.com/guides/openai.conversions_api_setup/generic\n- https://ispixelworking.com/guides/openai.pixel_setup/generic\n- https://ispixelworking.com/guides/tiktok.events_api_setup/generic\ndescription: Authentication methods for OpenAI Conversions API and TikTok Events API as described on IsPixelWorking pages.\nschemes:\n- type: http-bearer\n  name: OpenAI Conversions API key\n  evidence: 'Send a POST request to https://bzr.openai.com/v1/events?pid=<PIXEL-ID> with your Conversions API key as a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Provision it from the conversions tab in Ads Manager, or create it with your Advertiser API key (POST /v1/conversions/api_keys).\n- type: http-bearer\n  name: TikTok Access Token\n  evidence: 'Send events in a POST\
  \ request to https://business-api.tiktok.com/open_api/v1.3/event/track/ with the headers Access-Token: <your\n    token> and Content-Type: application/json .'\n  location: header\n  header: Access-Token\n  how_to_obtain: Generate an access token in Events Manager under the pixel Settings tab by clicking Generate Access Token.\nnote: No OAuth flows, API keys, or other authentication types are documented on the provided pages.\ndocs: https://ispixelworking.com/guides/openai.conversions_api_setup/generic\n"
source_yaml_url: https://artifacts.apis.io/ispixelworking-com/authentication/ispixelworking-com-authentication.yml
summary_line: 2 schemes
tags:
- Monitoring
- Web Tracking
---
