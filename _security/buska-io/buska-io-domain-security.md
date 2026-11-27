---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buska.io
  spf: true
hosts:
- cert_expires: Dec 27 17:09:47 2026 GMT
  host: buska.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buska Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buska, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Buska
provider_slug: buska-io
slug: buska-io-domain-security
source_filename: buska-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buska.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:09:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buska.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buska-io/security/buska-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Listening
- Lead Generation
- Artificial Intelligence
- B2B
- Marketing
---
