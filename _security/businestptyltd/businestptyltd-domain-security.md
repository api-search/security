---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enlight.io
  spf: false
hosts:
- cert_expires: Nov  9 23:39:32 2026 GMT
  host: businest.enlight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Businestptyltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Businestptyltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Businestptyltd
provider_slug: businestptyltd
slug: businestptyltd-domain-security
source_filename: businestptyltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: businest.enlight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:39:32 2026 GMT\n  hsts: false\ndomains:\n- domain: enlight.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/businestptyltd/refs/heads/main/security/businestptyltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting Training
- Advisory Services
- Bookkeeper Education
- Professional Development
- Revenue Growth
---
