---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moradas.dev
  spf: true
hosts:
- cert_expires: Jan 24 12:29:04 2027 GMT
  host: moradas.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moradas Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for moradas-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: moradas-dev
provider_slug: moradas-dev
slug: moradas-dev-domain-security
source_filename: moradas-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moradas.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 12:29:04 2027 GMT\n  hsts: false\ndomains:\n- domain: moradas.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/moradas-dev/security/moradas-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Address
- Portugal
- Autocomplete
- OpenAPI
- Free
---
