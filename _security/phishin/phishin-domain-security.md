---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: phish.in
  spf: true
hosts:
- cert_expires: Sep  7 12:39:22 2026 GMT
  host: phish.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phishin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phishin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Phishin
provider_slug: phishin
slug: phishin-domain-security
source_filename: phishin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phish.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:39:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: phish.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phishin/refs/heads/main/security/phishin-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Music
- Public APIs
---
