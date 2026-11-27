---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zyntra.app
  spf: true
hosts:
- cert_expires: Jan 14 19:15:12 2027 GMT
  host: zyntra.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zyntra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zyntra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Zyntra
provider_slug: zyntra-app
slug: zyntra-app-domain-security
source_filename: zyntra-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zyntra.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 19:15:12 2027 GMT\n  hsts: false\ndomains:\n- domain: zyntra.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zyntra-app/security/zyntra-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email Testing
- Automated Tests
- QA
- Password Reset
- Magic Link
---
