---
api_specs:
- filename: auctionfinder-fyi-v1-openapi.json
  format: json
  label: AuctionFinder API V1 API
  slug: auctionfinder-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctionfinder-fyi/openapi/_original/auctionfinder-fyi-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auctionfinder.fyi
  spf: true
hosts:
- cert_expires: Jan 19 18:05:46 2027 GMT
  host: auctionfinder.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AuctionFinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AuctionFinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AuctionFinder
provider_slug: auctionfinder-fyi
slug: auctionfinder-fyi-domain-security
source_filename: auctionfinder-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auctionfinder.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 18:05:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: auctionfinder.fyi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/auctionfinder-fyi/security/auctionfinder-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Auctions
- Data
- Open Data
---
