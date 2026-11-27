---
api_specs:
- filename: cityalert-live-agents-api-openapi.yml
  format: yaml
  label: CityAlert.live Agents API
  slug: cityalert-live-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-agents-api-openapi.yml
- filename: cityalert-live-community-api-openapi.yml
  format: yaml
  label: CityAlert.live Community API
  slug: cityalert-live-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-community-api-openapi.yml
- filename: cityalert-live-feeds-api-openapi.yml
  format: yaml
  label: CityAlert.live Feeds API
  slug: cityalert-live-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-feeds-api-openapi.yml
- filename: cityalert-live-history-api-openapi.yml
  format: yaml
  label: CityAlert.live History API
  slug: cityalert-live-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-history-api-openapi.yml
- filename: cityalert-live-incidents-api-openapi.yml
  format: yaml
  label: CityAlert.live Incidents API
  slug: cityalert-live-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-incidents-api-openapi.yml
- filename: cityalert-live-meta-api-openapi.yml
  format: yaml
  label: CityAlert.live Meta API
  slug: cityalert-live-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-meta-api-openapi.yml
- filename: cityalert-live-news-api-openapi.yml
  format: yaml
  label: CityAlert.live News API
  slug: cityalert-live-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-news-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cityalert.live
  spf: true
hosts:
- cert_expires: Dec 15 01:15:14 2026 GMT
  host: cityalert.live
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CityAlert.live Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CityAlert.live, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CityAlert.live
provider_slug: cityalert-live
slug: cityalert-live-domain-security
source_filename: cityalert-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cityalert.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 01:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: cityalert.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cityalert-live/security/cityalert-live-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Safety
- Mapping
- Real-Time
- Open Data
- Community
---
