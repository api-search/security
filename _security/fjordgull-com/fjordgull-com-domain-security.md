---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fjordgull.com
  spf: true
hosts:
- cert_expires: Dec  6 00:39:12 2026 GMT
  host: fjordgull.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fjordgull Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fjordgull, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fjordgull
provider_slug: fjordgull-com
slug: fjordgull-com-domain-security
source_filename: fjordgull-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fjordgull.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 00:39:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fjordgull.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fjordgull-com/security/fjordgull-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Supplements
- Omega-3
- Subscription
- Norway
---
