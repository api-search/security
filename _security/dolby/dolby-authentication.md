---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dolby-optiview-live-openapi.yml
  format: yaml
  label: Dolby OptiView Live
  slug: optiview-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-optiview-live-openapi.yml
- filename: dolby-millicast-api-openapi.yml
  format: yaml
  label: Dolby OptiView Real-time Streaming (Millicast)
  slug: real-time-millicast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-millicast-api-openapi.yml
- filename: dolby-millicast-director-openapi.yml
  format: yaml
  label: Dolby OptiView Director API (Millicast)
  slug: millicast-director
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-millicast-director-openapi.yml
- filename: dolby-millicast-analytics-openapi.yml
  format: yaml
  label: Dolby OptiView Advanced Analytics API (Millicast)
  slug: millicast-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-millicast-analytics-openapi.yml
- filename: dolby-optiview-ads-openapi.yml
  format: yaml
  label: Dolby OptiView Ads
  slug: optiview-ads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-optiview-ads-openapi.yml
- filename: dolby-optiview-ad-engine-openapi.yml
  format: yaml
  label: Dolby OptiView Ad Engine
  slug: optiview-ad-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/openapi/dolby-optiview-ad-engine-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Dolby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dolby secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dolby
provider_slug: dolby
scheme_count: 5
schemes:
- description: '### Usage

    #### Acquire secret from dashboard.

    * Login to the streaming dashboard

    * On the left menu, click on Settings

    * Navigate to the Security tab''s sub section API Secrets

    1. "+ Create" to generate a new named API Secret if needed

    2. Click on the copy button or the reveal button to access a previously created API Secret


    ![](../assets/api_secret.png "Find API Secret")'
  name: API_Secret
  scheme: bearer
  sources:
  - openapi/dolby-millicast-analytics-openapi.yml
  - openapi/dolby-millicast-api-openapi.yml
  - openapi/dolby-millicast-director-openapi.yml
  type: http
- description: API authentication token
  in: header
  name: ApiKeyAuth
  parameter: x-rasp-auth-token
  sources:
  - openapi/dolby-optiview-ad-engine-openapi.yml
  type: apiKey
- description: API key (username) and secret (password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dolby-optiview-ads-openapi.yml
  - openapi/dolby-optiview-live-openapi.yml
  type: http
- description: Organization identifier.
  in: header
  name: orgId
  parameter: x-org-id
  sources:
  - openapi/dolby-optiview-ads-openapi.yml
  type: apiKey
- in: header
  name: apiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/dolby-optiview-ads-signaling-v1-openapi.yml
  type: apiKey
slug: dolby-authentication
source_filename: dolby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/dolby-millicast-analytics-openapi.yml, openapi/dolby-millicast-api-openapi.yml,\n  openapi/dolby-millicast-director-openapi.yml, openapi/dolby-optiview-ad-engine-openapi.yml,\n  openapi/dolby-optiview-ads-openapi.yml, openapi/dolby-optiview-ads-signaling-v1-openapi.yml,\n  openapi/dolby-optiview-live-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: API_Secret\n  type: http\n  scheme: bearer\n  description: |-\n    ### Usage\n    #### Acquire secret from dashboard.\n    * Login to the streaming dashboard\n    * On the left menu, click on Settings\n    * Navigate to the Security tab's sub section API Secrets\n    1. \"+ Create\" to generate a new named API Secret if needed\n    2. Click on the copy button or the reveal button to access a previously created API Secret\n\n    ![](../assets/api_secret.png \"Find API Secret\")\n  sources:\n  - openapi/dolby-millicast-analytics-openapi.yml\n\
  \  - openapi/dolby-millicast-api-openapi.yml\n  - openapi/dolby-millicast-director-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-rasp-auth-token\n  description: API authentication token\n  sources:\n  - openapi/dolby-optiview-ad-engine-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API key (username) and secret (password).\n  sources:\n  - openapi/dolby-optiview-ads-openapi.yml\n  - openapi/dolby-optiview-live-openapi.yml\n- name: orgId\n  type: apiKey\n  in: header\n  parameter: x-org-id\n  description: Organization identifier.\n  sources:\n  - openapi/dolby-optiview-ads-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/dolby-optiview-ads-signaling-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/authentication/dolby-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Audio
- Video
- Streaming
- Media
- Real-Time
- WebRTC
- Advertising
- Video Player
- Live Streaming
- Broadcasting
---
