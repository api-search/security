---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lightyear.build
  spf: true
hosts:
- cert_expires: Dec 19 10:34:05 2026 GMT
  host: lightyear.build
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lightyear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightyear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lightyear
provider_slug: lightyear-build
slug: lightyear-build-domain-security
source_filename: lightyear-build-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightyear.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 10:34:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightyear.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lightyear-build/security/lightyear-build-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Artificial Intelligence
- Market Data
- Benchmarks
- Infrastructure
---
