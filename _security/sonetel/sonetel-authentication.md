---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sonetel-account-api-openapi.yml
  format: yaml
  label: Sonetel Account API
  slug: sonetel-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-account-api-openapi.yml
- filename: sonetel-ai-integration-api-openapi.yml
  format: yaml
  label: Sonetel Ai Integration API
  slug: sonetel-ai-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-ai-integration-api-openapi.yml
- filename: sonetel-ai-service-api-openapi.yml
  format: yaml
  label: Sonetel Ai Service API
  slug: sonetel-ai-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-ai-service-api-openapi.yml
- filename: sonetel-app-view-settings-api-openapi.yml
  format: yaml
  label: Sonetel App View Settings API
  slug: sonetel-app-view-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-app-view-settings-api-openapi.yml
- filename: sonetel-business-api-openapi.yml
  format: yaml
  label: Sonetel Business API
  slug: sonetel-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-business-api-openapi.yml
- filename: sonetel-call-recording-api-openapi.yml
  format: yaml
  label: Sonetel Call Recording API
  slug: sonetel-call-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-call-recording-api-openapi.yml
- filename: sonetel-country-api-openapi.yml
  format: yaml
  label: Sonetel Country API
  slug: sonetel-country-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-country-api-openapi.yml
- filename: sonetel-filemgr-api-openapi.yml
  format: yaml
  label: Sonetel Filemgr API
  slug: sonetel-filemgr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-filemgr-api-openapi.yml
- filename: sonetel-globaldata-api-openapi.yml
  format: yaml
  label: Sonetel Globaldata API
  slug: sonetel-globaldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-globaldata-api-openapi.yml
- filename: sonetel-internal-api-openapi.yml
  format: yaml
  label: Sonetel Internal API
  slug: sonetel-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-internal-api-openapi.yml
- filename: sonetel-make-calls-api-openapi.yml
  format: yaml
  label: Sonetel Make Calls API
  slug: sonetel-make-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-make-calls-api-openapi.yml
- filename: sonetel-numberstocksummary-api-openapi.yml
  format: yaml
  label: Sonetel Numberstocksummary API
  slug: sonetel-numberstocksummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-numberstocksummary-api-openapi.yml
- filename: sonetel-oauth-api-openapi.yml
  format: yaml
  label: Sonetel OAuth API
  slug: sonetel-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-oauth-api-openapi.yml
- filename: sonetel-prompt-api-openapi.yml
  format: yaml
  label: Sonetel Prompt API
  slug: sonetel-prompt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-prompt-api-openapi.yml
- filename: sonetel-textmgr-api-openapi.yml
  format: yaml
  label: Sonetel Textmgr API
  slug: sonetel-textmgr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-textmgr-api-openapi.yml
- filename: sonetel-transcription-api-openapi.yml
  format: yaml
  label: Sonetel Transcription API
  slug: sonetel-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-transcription-api-openapi.yml
- filename: sonetel-tts-api-openapi.yml
  format: yaml
  label: Sonetel Tts API
  slug: sonetel-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-tts-api-openapi.yml
- filename: sonetel-usage-api-openapi.yml
  format: yaml
  label: Sonetel Usage API
  slug: sonetel-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-usage-api-openapi.yml
- filename: sonetel-user-api-openapi.yml
  format: yaml
  label: Sonetel User API
  slug: sonetel-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/openapi/sonetel-user-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sonetel Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Sonetel secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Sonetel
provider_slug: sonetel
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: https://api.sonetel.com/SonetelAuth/beta/oauth/token
  name: Production
  sources:
  - openapi/sonetel-account-openapi.yml
  - openapi/sonetel-ai-business-openapi.yml
  - openapi/sonetel-ai-file-manager-openapi.yml
  - openapi/sonetel-ai-functions-openapi.yml
  - openapi/sonetel-ai-prompt-manager-openapi.yml
  - openapi/sonetel-ai-services-openapi.yml
  - openapi/sonetel-ai-text-manager-openapi.yml
  - openapi/sonetel-make-calls-openapi.yml
  - openapi/sonetel-recorded-calls-openapi.yml
  - openapi/sonetel-text-to-speech-openapi.yml
  - openapi/sonetel-transcription-openapi.yml
  - openapi/sonetel-usage-records-openapi.yml
  - openapi/sonetel-users-openapi.yml
  - openapi/sonetel-voice-apps-openapi.yml
  type: oauth2
slug: sonetel-authentication
source_filename: sonetel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://docs.sonetel.com/docs/sonetel-documentation/143990db3cda3-authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: Production\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.sonetel.com/SonetelAuth/beta/oauth/token\n    scopes: 0\n  sources:\n  - openapi/sonetel-account-openapi.yml\n  - openapi/sonetel-ai-business-openapi.yml\n  - openapi/sonetel-ai-file-manager-openapi.yml\n  - openapi/sonetel-ai-functions-openapi.yml\n  - openapi/sonetel-ai-prompt-manager-openapi.yml\n  - openapi/sonetel-ai-services-openapi.yml\n  - openapi/sonetel-ai-text-manager-openapi.yml\n  - openapi/sonetel-make-calls-openapi.yml\n  - openapi/sonetel-recorded-calls-openapi.yml\n  - openapi/sonetel-text-to-speech-openapi.yml\n  - openapi/sonetel-transcription-openapi.yml\n  - openapi/sonetel-usage-records-openapi.yml\n  - openapi/sonetel-users-openapi.yml\n  - openapi/sonetel-voice-apps-openapi.yml\n\
  derived_from: openapi/sonetel-account-openapi.yml, openapi/sonetel-ai-business-openapi.yml, openapi/sonetel-ai-file-manager-openapi.yml,\n  openapi/sonetel-ai-functions-openapi.yml, openapi/sonetel-ai-prompt-manager-openapi.yml, openapi/sonetel-ai-services-openapi.yml,\n  openapi/sonetel-ai-text-manager-openapi.yml, openapi/sonetel-make-calls-openapi.yml, openapi/sonetel-recorded-calls-openapi.yml,\n  openapi/sonetel-text-to-speech-openapi.yml, openapi/sonetel-transcription-openapi.yml, openapi/sonetel-usage-records-openapi.yml\n  ...\ndocs: https://docs.sonetel.com/docs/sonetel-documentation/143990db3cda3-authentication\ndocumented:\n  token_endpoint: https://api.sonetel.com/SonetelAuth/oauth/token\n  grant_types:\n  - password\n  - refresh_token\n  client_authentication: HTTP Basic with sonetel-api as the username as well as the password\n  credentials: Sonetel account email address and password sent in the request body\n  token_type: bearer\n  token_lifetime_text: Access tokens are\
  \ valid for 30 days. Use the refresh_token to generate a new access token.\n  refresh: Include the parameter refresh=yes when sending a request to /oauth/token to receive a refresh_token in the response.\n  usage: 'Authorization: Bearer <ACCESS_TOKEN>'\n  notes: Docs show the token endpoint at /SonetelAuth/oauth/token while the spec tokenUrl is /SonetelAuth/beta/oauth/token;\n    no client-credentials or per-application keys are documented, the API authenticates as the Sonetel user.\nfaq: https://docs.sonetel.com/docs/sonetel-documentation/862afa73a11f1-frequently-asked-questions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonetel/refs/heads/main/authentication/sonetel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Telephony
- Phone Numbers
- VoIP
- Communications
- SMS
- Call Recording
- Small Business
---
