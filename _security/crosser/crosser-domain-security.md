---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crosser.io
  spf: true
hosts:
- cert_expires: Apr 13 23:59:59 2027 GMT
  host: crosser.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crosser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crosser - IoT Edge Streaming Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crosser - IoT Edge Streaming Analytics
provider_slug: crosser
slug: crosser-domain-security
source_filename: crosser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crosser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: crosser.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/crosser/security/crosser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IoT
- Edge-Computing
- Streaming-Analytics
- Industrial
---
