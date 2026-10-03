---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bima.om
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: bima.om
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bima Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BIMA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BIMA
provider_slug: bima
slug: bima-domain-security
source_filename: bima-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bima.om\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bima.om\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bima/refs/heads/main/security/bima-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Insurance
- Oman
- Digital
- Gateways
- Bima
---
