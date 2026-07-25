---
api_key_in:
- query
- body
api_specs:
- filename: vbout-account-api-openapi.yml
  format: yaml
  label: VBOUT Account API
  slug: vbout-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-account-api-openapi.yml
- filename: vbout-aichatbot-api-openapi.yml
  format: yaml
  label: VBOUT AIchatbot API
  slug: vbout-aichatbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-aichatbot-api-openapi.yml
- filename: vbout-application-api-openapi.yml
  format: yaml
  label: VBOUT Application API
  slug: vbout-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-application-api-openapi.yml
- filename: vbout-automation-api-openapi.yml
  format: yaml
  label: VBOUT Automation API
  slug: vbout-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-automation-api-openapi.yml
- filename: vbout-contact-api-openapi.yml
  format: yaml
  label: VBOUT Contact API
  slug: vbout-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-contact-api-openapi.yml
- filename: vbout-email-marketing-api-openapi.yml
  format: yaml
  label: VBOUT Email Marketing API
  slug: vbout-email-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-email-marketing-api-openapi.yml
- filename: vbout-emailmarketing-api-openapi.yml
  format: yaml
  label: VBOUT EmailMarketing API
  slug: vbout-emailmarketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-emailmarketing-api-openapi.yml
- filename: vbout-goals-api-openapi.yml
  format: yaml
  label: VBOUT Goals API
  slug: vbout-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-goals-api-openapi.yml
- filename: vbout-help-api-openapi.yml
  format: yaml
  label: VBOUT Help API
  slug: vbout-help-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-help-api-openapi.yml
- filename: vbout-pipeline-api-openapi.yml
  format: yaml
  label: VBOUT Pipeline API
  slug: vbout-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-pipeline-api-openapi.yml
- filename: vbout-popups-api-openapi.yml
  format: yaml
  label: VBOUT Popups API
  slug: vbout-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-popups-api-openapi.yml
- filename: vbout-settings-api-openapi.yml
  format: yaml
  label: VBOUT Settings API
  slug: vbout-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-settings-api-openapi.yml
- filename: vbout-social-media-api-openapi.yml
  format: yaml
  label: VBOUT Social Media API
  slug: vbout-social-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-social-media-api-openapi.yml
- filename: vbout-socialmedia-api-openapi.yml
  format: yaml
  label: VBOUT SocialMedia API
  slug: vbout-socialmedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-socialmedia-api-openapi.yml
- filename: vbout-users-workflow-api-openapi.yml
  format: yaml
  label: VBOUT Users & Workflow API
  slug: vbout-users-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-users-workflow-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: VBOUT API authentication profile. The API authenticates every call with a single account-level API key. The published OpenAPI (3.1.0, harvested from https://developers.vbout.com/scripts/openapi.json) declares no components.securitySchemes, so this profile is captured from the developer quickstart, the legacy Swagger console, and the live /.well-known/ai-plugin.json manifest on www.vbout.com.
kind: authentication
layout: security
method: searched
name: Vbout Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: VBOUT secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: VBOUT
provider_slug: vbout
scheme_count: 2
schemes:
- description: 'A unique user API key generated from Account Settings. Passed as the `key` parameter — the quickstart shows it in a JSON request body ({"key":"YOUR_API_ID"}) and the legacy API console adds it as an `api_key`/`key` query parameter. Two key types exist: a User Key (generated directly from Account Settings) and an Application Key (generated from Account Settings and activated through VBOUT Connect for third-party apps).'
  in: query
  name: api_key
  parameter: key
  sources:
  - https://developers.vbout.com/quickstart
  - https://developers.vbout.com/console
  type: apiKey
- description: OAuth authorization surface used by third-party applications (VBOUT Connect) and the published ChatGPT plugin manifest. The live /.well-known/ai-plugin.json on www.vbout.com declares auth type "oauth" with client_url https://app.vbout.com/Login and authorization_url https://app.vbout.com/Authorize, with an empty scope string. No public scope catalog or token-endpoint documentation was found.
  flows:
  - authorizationUrl: https://app.vbout.com/Authorize
    flow: authorizationCode
  name: vbout_connect_oauth
  sources:
  - https://www.vbout.com/.well-known/ai-plugin.json
  type: oauth2
slug: vbout-authentication
source_filename: vbout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.vbout.com/quickstart\ndocs: https://developers.vbout.com/quickstart\ndescription: >-\n  VBOUT API authentication profile. The API authenticates every call with a\n  single account-level API key. The published OpenAPI (3.1.0, harvested from\n  https://developers.vbout.com/scripts/openapi.json) declares no\n  components.securitySchemes, so this profile is captured from the developer\n  quickstart, the legacy Swagger console, and the live /.well-known/ai-plugin.json\n  manifest on www.vbout.com.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [query, body]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: api_key\n    type: apiKey\n    in: query\n    parameter: key\n    description: >-\n      A unique user API key generated from Account Settings. Passed as the\n      `key` parameter — the quickstart shows it in a JSON request body\n      ({\"key\":\"YOUR_API_ID\"}) and the legacy API console adds\
  \ it as an\n      `api_key`/`key` query parameter. Two key types exist: a User Key\n      (generated directly from Account Settings) and an Application Key\n      (generated from Account Settings and activated through VBOUT Connect\n      for third-party apps).\n    sources:\n      - https://developers.vbout.com/quickstart\n      - https://developers.vbout.com/console\n  - name: vbout_connect_oauth\n    type: oauth2\n    description: >-\n      OAuth authorization surface used by third-party applications (VBOUT\n      Connect) and the published ChatGPT plugin manifest. The live\n      /.well-known/ai-plugin.json on www.vbout.com declares auth type \"oauth\"\n      with client_url https://app.vbout.com/Login and authorization_url\n      https://app.vbout.com/Authorize, with an empty scope string. No public\n      scope catalog or token-endpoint documentation was found.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.vbout.com/Authorize\n    sources:\n\
  \      - https://www.vbout.com/.well-known/ai-plugin.json\nerrors:\n  missing_or_invalid_key:\n    http_status: 401\n    envelope:\n      response:\n        header: {status: error, dataType: array}\n        data: {errorCode: 1000, errorMessage: Missing or Invalid authentication key.}\n    observed: '2026-07-21 — live response from https://api.vbout.com/1/apidocs.json with no key'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/authentication/vbout-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Marketing Automation
- Email Marketing
- Social Media
- Lead Management
- Landing Pages
- Chatbots
- Contacts
- Campaigns
- SaaS
---
