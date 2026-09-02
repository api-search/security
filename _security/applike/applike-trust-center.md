---
api_specs:
- filename: applike-app-partner-connection-api-openapi.yml
  format: yaml
  label: AppLike Group App Partner Connection API
  slug: applike-app-partner-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-app-partner-connection-api-openapi.yml
- filename: applike-appevents-api-openapi.yml
  format: yaml
  label: AppLike Group Appevents API
  slug: applike-appevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-appevents-api-openapi.yml
- filename: applike-apps-api-openapi.yml
  format: yaml
  label: AppLike Group Apps API
  slug: applike-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-apps-api-openapi.yml
- filename: applike-bids-api-openapi.yml
  format: yaml
  label: AppLike Group Bids API
  slug: applike-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-bids-api-openapi.yml
- filename: applike-campaigns-api-openapi.yml
  format: yaml
  label: AppLike Group Campaigns API
  slug: applike-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-campaigns-api-openapi.yml
- filename: applike-partner-configurations-api-openapi.yml
  format: yaml
  label: AppLike Group Partner Configurations API
  slug: applike-partner-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-partner-configurations-api-openapi.yml
- filename: applike-partners-api-openapi.yml
  format: yaml
  label: AppLike Group Partners API
  slug: applike-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-partners-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Applike Trust Center
name_suffix: Trust Center
overview: AppLike Group maintains a public trust center covering its security and compliance posture.
provider_name: AppLike Group
provider_slug: applike
slug: applike-trust-center
source_filename: applike-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://justtrack.io/security/, https://adjoe.io/\nnote: >-\n  Neither brand runs a hosted trust center (no trust.<domain>, no Vanta/Drata/SafeBase portal, no downloadable audit\n  report). What exists is a marketing security page per brand naming one certification each. probe-security-programs.py\n  returned trust=none because it probes only the hosts declared in apis.yml + OpenAPI servers; the pages below were\n  found by reading each brand's own footer.\ntrust_pages:\n- brand: justtrack\n  url: https://justtrack.io/security/\n  http_status: 200\n  certifications:\n  - name: ISO/IEC 27001:2022\n    scope: information security management system\n    statement: >-\n      \"justtrack maintains ISO/IEC 27001:2022 certification for the information security management system.\"\n    certificate_published: false\n    auditor_named: false\n  claims:\n  - >-\n      \"We are dedicated to maintaining the highest standards of data security,\
  \ user privacy, and global regulatory\n      adherence.\"\n- brand: adjoe\n  url: https://adjoe.io/\n  http_status: 200\n  certifications:\n  - name: ISO 27001\n    scope: not stated\n    statement: >-\n      \"adjoe holds the ISO 27001 certification, the most recognized international standard for protecting\n      information. This confirms that security is a non-negotiable component engineered into every layer of our\n      complete technology environment.\"\n    certificate_published: false\n    auditor_named: false\n    version_specified: false\n  note: >-\n    The claim sits in a homepage section headed \"Security Engineered In. Certified Worldwide.\" There is no dedicated\n    adjoe security or trust page; /trust-center returns 404 and trust.adjoe.io does not resolve.\ndata_protection:\n- brand: justtrack\n  dpa: https://justtrack.io/dpa/\n  privacy_notice: https://justtrack.io/privacy-notice/\n  sdk_privacy_controls: https://docs.justtrack.io/sdk/privacy/\n  detail: >-\n    The\
  \ SDK documents manual-start, stop-tracking and anonymize controls so publishers can gate collection on user\n    consent — a real, documented consent surface for a company whose product is mobile attribution.\n- brand: adjoe\n  privacy: https://adjoe.io/privacy/\n  google_play_data_safety: https://docs.adjoe.io/rewarded-solutions/playtime-sdk-integration/android/google-play-data-safety-guidance\nabsent:\n  soc2: not claimed by either brand\n  pci_dss: not applicable / not claimed\n  hipaa: not applicable\n  fedramp: not applicable\n  penetration_test_summary: not published\n  subprocessor_list: not found on a public page\n  status_of_certificates: >-\n    Neither brand publishes the certificate itself, the certification body, the certificate number or the scope\n    statement — the ISO 27001 claim is unverifiable from the public surface on both sides.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/security/applike-trust-center.yml
summary_line: trust center published
tags:
- Mobile Attribution
- User Acquisition
- AdTech
- Mobile Advertising
- App Monetization
- rewarded-advertising
- Mobile SDK
- Mobile Analytics
- Marketing Attribution
- Mobile Games
- Event Tracking
- Company
trust_url: ''
---
