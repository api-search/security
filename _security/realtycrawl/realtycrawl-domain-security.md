---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: realtycrawl.dev
  spf: false
hosts:
- cert_expires: Jan 12 06:27:07 2027 GMT
  host: realtycrawl.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RealtyCrawl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealtyCrawl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RealtyCrawl
provider_slug: realtycrawl
slug: realtycrawl-domain-security
source_filename: realtycrawl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realtycrawl.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 06:27:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: realtycrawl.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/realtycrawl/security/realtycrawl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Real Estate
- Data
- Listings
- Aggregation
- Company
---
