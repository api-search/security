---
api_specs:
- filename: appstorespy-app-store-api-openapi.yml
  format: yaml
  label: AppstoreSpy App Store API
  slug: appstorespy-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-app-store-api-openapi.yml
- filename: appstorespy-events-api-openapi.yml
  format: yaml
  label: AppstoreSpy Events API
  slug: appstorespy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-events-api-openapi.yml
- filename: appstorespy-google-play-api-openapi.yml
  format: yaml
  label: AppstoreSpy Google Play API
  slug: appstorespy-google-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-google-play-api-openapi.yml
- filename: appstorespy-jobs-api-openapi.yml
  format: yaml
  label: AppstoreSpy Jobs API
  slug: appstorespy-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-jobs-api-openapi.yml
- filename: appstorespy-search-filter-v-2-api-openapi.yml
  format: yaml
  label: AppstoreSpy Search Filter v.2 API
  slug: appstorespy-search-filter-v-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-search-filter-v-2-api-openapi.yml
- filename: appstorespy-suggestions-api-openapi.yml
  format: yaml
  label: AppstoreSpy Suggestions API
  slug: appstorespy-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-suggestions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: appstorespy.com
  spf: true
hosts:
- cert_expires: Oct 23 01:45:34 2026 GMT
  host: api.appstorespy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appstorespy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppstoreSpy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AppstoreSpy
provider_slug: appstorespy
slug: appstorespy-domain-security
source_filename: appstorespy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.appstorespy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 01:45:34 2026 GMT\n  hsts: false\ndomains:\n- domain: appstorespy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/security/appstorespy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Mobile Apps
- App Store Optimization
- Market Intelligence
- App Analytics
- Google Play
- apple-app-store
- Reviews and Ratings
- download-revenue-estimates
- Marketing
---
