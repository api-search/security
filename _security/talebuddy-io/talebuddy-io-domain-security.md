---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: talebuddy.io
  spf: false
hosts:
- cert_expires: Feb 17 11:24:53 2027 GMT
  host: talebuddy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Talebuddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talebuddy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Talebuddy
provider_slug: talebuddy-io
slug: talebuddy-io-domain-security
source_filename: talebuddy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talebuddy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 11:24:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talebuddy.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/talebuddy-io/security/talebuddy-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Writing
- AI
- Storytelling
- AuthorTools
- Companion
---
