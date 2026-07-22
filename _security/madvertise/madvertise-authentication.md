---
api_key_in: []
auth_types:
- placement-code
- app-id
description: ''
kind: authentication
layout: security
method: searched
name: Madvertise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Madvertise secures its APIs with placement-code and app-id across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Madvertise
provider_slug: madvertise
scheme_count: 2
schemes:
- detail: Ad requests carry the zone/publisher/placement ID in the `s` query parameter (mobile.mng-ads.com) or the URL path (/bidrequest/{placement_code}). This identifies inventory, not an authenticated principal.
  location: query-or-path
  name: placement-code
  source: https://developers.bluestack.app/adserving/ad-request-api-documentation
  type: identifier
- detail: Mobile SDKs initialize with a publisher appID via MobileAds.sharedInstance() (iOS) / SDK init (Android) before loading ads.
  location: sdk-init
  name: app-id
  source: https://developers.bluestack.app/ios/
  type: identifier
slug: madvertise-authentication
source_filename: madvertise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://developers.bluestack.app/adserving/ad-request-api-documentation,\n  https://developers.bluestack.app/adserving/open-rtb-bid-request-api,\n  https://developers.bluestack.app/android/\nnote: >-\n  No OpenAPI is published, so this profile is captured from the developer docs\n  rather than derived. The ad-serving APIs are not key/token authenticated;\n  callers are identified by placement/publisher codes.\nsummary:\n  types: [placement-code, app-id]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: placement-code\n  type: identifier\n  location: query-or-path\n  detail: >-\n    Ad requests carry the zone/publisher/placement ID in the `s` query parameter\n    (mobile.mng-ads.com) or the URL path (/bidrequest/{placement_code}). This\n    identifies inventory, not an authenticated principal.\n  source: https://developers.bluestack.app/adserving/ad-request-api-documentation\n- name: app-id\n  type: identifier\n\
  \  location: sdk-init\n  detail: >-\n    Mobile SDKs initialize with a publisher appID via MobileAds.sharedInstance()\n    (iOS) / SDK init (Android) before loading ads.\n  source: https://developers.bluestack.app/ios/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madvertise/refs/heads/main/authentication/madvertise-authentication.yml
summary_line: placement-code/app-id · 2 schemes
tags:
- Company
- Advertising
- AdTech
- Mobile
- Monetization
- Programmatic
- OpenRTB
- SDK
- Publishers
---
