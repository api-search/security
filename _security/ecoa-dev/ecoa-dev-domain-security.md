---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecoa.dev
  spf: true
hosts:
- cert_expires: Jan  3 03:29:02 2027 GMT
  host: ecoa.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ecoa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ecoa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ecoa
provider_slug: ecoa-dev
slug: ecoa-dev-domain-security
source_filename: ecoa-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecoa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 03:29:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ecoa.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecoa-dev/security/ecoa-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Privacy
- Compliance
- AppTesting
- Low-Code
---
