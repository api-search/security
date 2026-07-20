---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Channelengine Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChannelEngine secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ChannelEngine
provider_slug: channelengine
scheme_count: 1
schemes:
- apis:
  - Merchant API
  - Channel API
  - Channel Management API
  description: All Merchant API and Channel API calls are authenticated with a per-tenant API key passed as the `apikey` query parameter. Generate the key in the ChannelEngine web app under Settings > Merchant API keys. ChannelEngine warns that passing the key in the URL can be logged by intermediaries, so treat keys as secrets and rotate as needed. The base URL is https://{subdomain}.channelengine.net/api (append your tenant subdomain).
  in: query
  name: ApiKeyAuth
  parameter: apikey
  type: apiKey
slug: channelengine-authentication
source_filename: channelengine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://support.channelengine.com/hc/en-us/articles/4409515268637-Merchant-API-before-you-start\ndocs: https://support.channelengine.com/hc/en-us/articles/32426668116125-ChannelEngine-get-API-access\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  api_key_name: apikey\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: >-\n    All Merchant API and Channel API calls are authenticated with a per-tenant\n    API key passed as the `apikey` query parameter. Generate the key in the\n    ChannelEngine web app under Settings > Merchant API keys. ChannelEngine\n    warns that passing the key in the URL can be logged by intermediaries, so\n    treat keys as secrets and rotate as needed. The base URL is\n    https://{subdomain}.channelengine.net/api (append your tenant subdomain).\n  apis: [Merchant API, Channel API, Channel Management API]\nplatform_sso:\n  note: >-\n\
  \    Distinct from API-key data access, the ChannelEngine web application is\n    secured by an OpenID Connect identity provider at login.channelengine.net.\n    This is not used to call the data APIs.\n  issuer: https://login.channelengine.net/\n  grant_types: [client_credentials, authorization_code, refresh_token]\n  scopes: [openid, offline_access, email, roles, profile, permissions]\n  discovery: well-known/channelengine-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelengine/refs/heads/main/authentication/channelengine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- E-commerce
- Marketplace Integration
- Multichannel Commerce
- Order Management
- Inventory Management
- Product Information
- Retail
- Webhooks
- Netherlands
---
