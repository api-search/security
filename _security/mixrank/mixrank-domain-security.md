---
api_specs:
- filename: mixrank-account-api-openapi.yml
  format: yaml
  label: MixRank Account API
  slug: mixrank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-account-api-openapi.yml
- filename: mixrank-audience-segments-api-openapi.yml
  format: yaml
  label: MixRank Audience Segments API
  slug: mixrank-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-audience-segments-api-openapi.yml
- filename: mixrank-companies-api-openapi.yml
  format: yaml
  label: MixRank Companies API
  slug: mixrank-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-companies-api-openapi.yml
- filename: mixrank-email-api-openapi.yml
  format: yaml
  label: MixRank Email API
  slug: mixrank-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-email-api-openapi.yml
- filename: mixrank-ios-app-privacy-api-openapi.yml
  format: yaml
  label: MixRank iOS App Privacy API
  slug: mixrank-ios-app-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-app-privacy-api-openapi.yml
- filename: mixrank-ios-apps-api-openapi.yml
  format: yaml
  label: MixRank iOS Apps API
  slug: mixrank-ios-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-apps-api-openapi.yml
- filename: mixrank-ios-developers-api-openapi.yml
  format: yaml
  label: MixRank iOS Developers API
  slug: mixrank-ios-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-developers-api-openapi.yml
- filename: mixrank-ios-rankings-api-openapi.yml
  format: yaml
  label: MixRank iOS Rankings API
  slug: mixrank-ios-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-rankings-api-openapi.yml
- filename: mixrank-ios-sdks-api-openapi.yml
  format: yaml
  label: MixRank iOS SDKs API
  slug: mixrank-ios-sdks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-sdks-api-openapi.yml
- filename: mixrank-people-api-openapi.yml
  format: yaml
  label: MixRank People API
  slug: mixrank-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-people-api-openapi.yml
- filename: mixrank-play-store-apps-api-openapi.yml
  format: yaml
  label: MixRank Play Store Apps API
  slug: mixrank-play-store-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-apps-api-openapi.yml
- filename: mixrank-play-store-developers-api-openapi.yml
  format: yaml
  label: MixRank Play Store Developers API
  slug: mixrank-play-store-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-developers-api-openapi.yml
- filename: mixrank-play-store-rankings-api-openapi.yml
  format: yaml
  label: MixRank Play Store Rankings API
  slug: mixrank-play-store-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-rankings-api-openapi.yml
- filename: mixrank-play-store-sdks-api-openapi.yml
  format: yaml
  label: MixRank Play Store SDKs API
  slug: mixrank-play-store-sdks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-sdks-api-openapi.yml
- filename: mixrank-web-tags-api-openapi.yml
  format: yaml
  label: MixRank Web Tags API
  slug: mixrank-web-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-web-tags-api-openapi.yml
- filename: mixrank-websites-api-openapi.yml
  format: yaml
  label: MixRank Websites API
  slug: mixrank-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-websites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mixrank.com
  spf: true
hosts:
- cert_expires: Sep 29 23:18:46 2026 GMT
  host: mixrank.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:18:33 2026 GMT
  host: api.mixrank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mixrank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MixRank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MixRank
provider_slug: mixrank
slug: mixrank-domain-security
source_filename: mixrank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mixrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:18:46 2026 GMT\n  hsts: false\n- host: api.mixrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:18:33 2026 GMT\n  hsts: null\ndomains:\n- domain: mixrank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/security/mixrank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Technographics
- Firmographics
- People Data
- Mobile Apps
- SDK Intelligence
- App Store
- Web Technology
- Sales Intelligence
- Data Enrichment
---
