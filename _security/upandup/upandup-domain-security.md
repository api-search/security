---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upandup.co
  spf: true
hosts:
- cert_expires: Sep 29 03:29:30 2026 GMT
  host: upandup.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upandup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Up&Up, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Up&Up
provider_slug: upandup
slug: upandup-domain-security
source_filename: upandup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upandup.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upandup.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upandup/refs/heads/main/security/upandup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Rentals
- PropTech
- Housing
- FinTech
- Homeownership
---
