---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Digimarc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digimarc declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Digimarc
provider_slug: digimarc
scheme_count: 2
schemes:
- applies_to:
  - digimarc:illuminate-mobile-rest-api
  description: Illuminate Mobile API key, created by an Account Administrator in the Illuminate UI. "The Mobile API keys have read-only (MOBILE_READ_ONLY) permissions." Included in the Authorization header of every request to https://api.dmrc.app/api/v1.
  format: 'Authorization: ApiKey $API_KEY'
  header: Authorization
  in: header
  name: ApiKey
  permissions:
  - MOBILE_READ_ONLY
  type: apiKey
- description: The Digimarc Mobile SDK requires a license key generated in the Digimarc Print & Audio Module or Illuminate, set via Info.plist, DMSLicenseManager, or reader options (iOS) / app configuration (Android). Since DM SDK 4.0.1 the SDK additionally requires an Illuminate Mobile API Key and Account ID to resolve watermarks.
  docs:
  - https://landing.digimarc.com/mobile-sdk/documentation/iOS/installation-guide.html
  - https://landing.digimarc.com/mobile-sdk/documentation/android/javadoc/reference/getting-started.html
  name: DM SDK license key
  type: license-key
slug: digimarc-authentication
source_filename: digimarc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Digimarc authentication\ngenerated: '2026-11-05'\nmethod: searched\nsource: https://github.com/digimarc-corp/illuminate-mobile-rest-api/blob/main/README.md\ndocs: https://github.com/digimarc-corp/illuminate-mobile-rest-api/blob/main/README.md\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  header: Authorization\n  format: 'Authorization: ApiKey $API_KEY'\n  description: Illuminate Mobile API key, created by an Account Administrator in the Illuminate UI. \"The Mobile API keys have read-only (MOBILE_READ_ONLY) permissions.\" Included in the Authorization header of every request to https://api.dmrc.app/api/v1.\n  permissions:\n  - MOBILE_READ_ONLY\n  applies_to:\n  - digimarc:illuminate-mobile-rest-api\n- name: DM SDK license key\n  type: license-key\n  description: The Digimarc Mobile SDK requires a license key generated in the Digimarc Print & Audio Module or Illuminate, set via Info.plist, DMSLicenseManager, or reader options (iOS) / app configuration (Android).\
  \ Since DM SDK 4.0.1 the SDK additionally requires an Illuminate Mobile API Key and Account ID to resolve watermarks.\n  docs:\n  - https://landing.digimarc.com/mobile-sdk/documentation/iOS/installation-guide.html\n  - https://landing.digimarc.com/mobile-sdk/documentation/android/javadoc/reference/getting-started.html\nnotes: Mobile API keys are available only for supported subscriptions (Android Getting Started). No OAuth is documented.\n"
source_yaml_url: https://artifacts.apis.io/digimarc/authentication/digimarc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Digital Watermarking
- Product Authentication
- Anti-Counterfeiting
- Connected Packaging
- QR Codes
- Content Provenance
- Mobile SDK
---
