---
anonymous_access: false
api_key_in: []
auth_types: []
description: deepidv uses API keys to authenticate every request. Pass your secret key via HTTP header — missing or invalid keys return a 401 error.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deepidv Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deep Identity Inc. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Deep Identity Inc.
provider_slug: deepidv-com
scheme_count: 1
schemes:
- evidence: deepidv uses API keys to authenticate every request. Pass your secret key via HTTP header — missing or invalid keys return a 401 error.
  header: x-api-key
  how_to_obtain: Generate a key from the API Authentication page or in the deepidv Admin Console under Settings → API Keys.
  location: header
  name: API Key
  type: apiKey
slug: deepidv-com-authentication
source_filename: deepidv-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.deepidv.com/authentication
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.deepidv.com/authentication\nsources:\n- https://docs.deepidv.com/authentication\n- https://docs.deepidv.com/integrate/sdks/typescript/server/authentication\n- https://www.deepidv.com/media/articles/voice-biometrics-authentication-deepfake-audio-threat\n- https://www.deepidv.com/media/articles/palm-vein-biometrics-contactless-authentication-emerging\ndescription: deepidv uses API keys to authenticate every request. Pass your secret key via HTTP header — missing or invalid keys return a 401\n  error.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: deepidv uses API keys to authenticate every request. Pass your secret key via HTTP header — missing or invalid keys return a 401 error.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate a key from the API Authentication page or in the deepidv Admin Console under Settings → API Keys.\nnote: No OAuth2,\
  \ HTTP basic, bearer, JWT, HMAC, MTLS, or other schemes are documented on the provided pages.\ndocs: https://docs.deepidv.com/authentication\n"
source_yaml_url: https://artifacts.apis.io/deepidv-com/authentication/deepidv-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Identity Verification
- Fraud Prevention
- Biometrics
- Deepfake Detection
---
