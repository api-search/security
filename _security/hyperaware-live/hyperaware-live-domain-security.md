---
api_specs:
- filename: hyperaware-live-trends-api-openapi.yml
  format: yaml
  label: Hyperaware Trends API
  slug: hyperaware-live-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperaware-live/openapi/hyperaware-live-trends-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperaware.live
  spf: true
hosts:
- cert_expires: Dec 22 15:25:19 2026 GMT
  host: hyperaware.live
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hyperaware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperaware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyperaware
provider_slug: hyperaware-live
slug: hyperaware-live-domain-security
source_filename: hyperaware-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperaware.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 15:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hyperaware.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hyperaware-live/security/hyperaware-live-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trending
- Aggregator
- Data
---
