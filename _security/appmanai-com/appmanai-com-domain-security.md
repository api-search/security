---
api_specs:
- filename: appmanai-com-app-metadata-api-openapi.yml
  format: yaml
  label: AppManAi App Metadata API
  slug: appmanai-com-app-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-metadata-api-openapi.yml
- filename: appmanai-com-app-metrics-api-openapi.yml
  format: yaml
  label: AppManAi App Metrics API
  slug: appmanai-com-app-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-metrics-api-openapi.yml
- filename: appmanai-com-app-reviews-api-openapi.yml
  format: yaml
  label: AppManAi App Reviews API
  slug: appmanai-com-app-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-reviews-api-openapi.yml
- filename: appmanai-com-app-search-api-openapi.yml
  format: yaml
  label: AppManAi App Search API
  slug: appmanai-com-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appmanai.com
  spf: true
hosts:
- cert_expires: Dec  8 07:47:57 2026 GMT
  host: appmanai.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AppManAi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppManAi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AppManAi
provider_slug: appmanai-com
slug: appmanai-com-domain-security
source_filename: appmanai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appmanai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 07:47:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: appmanai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/appmanai-com/security/appmanai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- App Store Data
- Google Play Data
- ASO
- Data API
- App Intelligence
---
