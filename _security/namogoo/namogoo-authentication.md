---
api_key_in:
- application-manifest
- sdk-initialization
auth_types:
- account-id
description: ''
kind: authentication
layout: security
method: searched
name: Namogoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Namogoo secures its APIs with account-id across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Namogoo
provider_slug: namogoo
scheme_count: 2
schemes:
- description: 'Android: a meta-data entry in AndroidManifest.xml carrying the Wandz.ai Account ID, read by WandzClient.start(applicationContext) at SDK initialization.'
  in: application-manifest
  issued_via: https://wandz.ai/contact-us/
  name: wandz-account-id
  parameter: ai.wandz.sdk.client_id
  portal: https://app.wandz.ai/login
  sources:
  - https://github.com/namogoo/wandz-android-sdk
  type: apiKey
- description: iOS Intent-Based Promotions SDK (NamogooIBPSDK, CocoaPods) is initialized with a Namogoo-issued account identifier; the value is provisioned by Namogoo, not self-service.
  in: sdk-initialization
  name: namogoo-ibp-account-id
  sources:
  - https://github.com/namogoo/namogoo-ibp-ios-sdk
  type: apiKey
slug: namogoo-authentication
source_filename: namogoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://github.com/namogoo/wandz-android-sdk\ndocs: https://github.com/namogoo/wandz-android-sample/raw/main/ReadmeAssets/WandzAndroidSDK.pdf\nnote: >-\n  DERIVED FROM SDK DOCUMENTATION, NOT FROM AN OPENAPI. Namogoo / Wandz.ai publishes no OpenAPI\n  or public REST reference, so there are no securitySchemes to aggregate. The only documented\n  authentication model is the tenant Account ID (client ID) that activates the SDK against the\n  Wandz.ai platform; the Account ID is issued by the vendor after a sales conversation and the\n  server-side credential model is not published.\nsummary:\n  types: [account-id]\n  api_key_in: [application-manifest, sdk-initialization]\n  oauth2_flows: []\n  public_rest_api: false\nschemes:\n- name: wandz-account-id\n  type: apiKey\n  in: application-manifest\n  parameter: ai.wandz.sdk.client_id\n  description: >-\n    Android: a meta-data entry in AndroidManifest.xml carrying the Wandz.ai Account\
  \ ID, read by\n    WandzClient.start(applicationContext) at SDK initialization.\n  issued_via: https://wandz.ai/contact-us/\n  portal: https://app.wandz.ai/login\n  sources: [https://github.com/namogoo/wandz-android-sdk]\n- name: namogoo-ibp-account-id\n  type: apiKey\n  in: sdk-initialization\n  description: >-\n    iOS Intent-Based Promotions SDK (NamogooIBPSDK, CocoaPods) is initialized with a\n    Namogoo-issued account identifier; the value is provisioned by Namogoo, not self-service.\n  sources: [https://github.com/namogoo/namogoo-ibp-ios-sdk]\ngaps:\n- No public REST/GraphQL endpoint, so no bearer/OAuth2/OIDC scheme is documented anywhere public.\n- No self-service key issuance — credentials are provisioned through a contact-sales flow.\n- The full SDK reference is a 3.7 MB PDF in a GitHub repository, not a web reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namogoo/refs/heads/main/authentication/namogoo-authentication.yml
summary_line: account-id · 2 schemes
tags:
- Company
- E-Commerce
- Retail
- Personalization
- Customer Experience
- Predictive AI
- Marketing
- Mobile SDK
- Israel
---
