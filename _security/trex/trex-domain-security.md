---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trex.com
  spf: true
hosts:
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: www.trex.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.trex.com
  https: false
- host: api.trex.com
  https: false
kind: domain-security
layout: security
method: probed
name: Trex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trex Company, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trex Company
provider_slug: trex
slug: trex-domain-security
source_filename: trex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.trex.com\n  https: false\n- host: api.trex.com\n  https: false\ndomains:\n- domain: trex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trex/refs/heads/main/security/trex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Composite Decking
- Outdoor
- Building Products
---
