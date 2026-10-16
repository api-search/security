---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: banxico.org.mx
  spf: true
hosts:
- cert_expires: Nov  8 02:01:00 2026 GMT
  host: www.banxico.org.mx
  hsts: true
  hsts_max_age: 480
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Banco De Mexico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banco de Mexico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Banco de Mexico
provider_slug: banco-de-mexico
slug: banco-de-mexico-domain-security
source_filename: banco-de-mexico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.banxico.org.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 02:01:00 2026 GMT\n  hsts: true\n  hsts_max_age: 480\ndomains:\n- domain: banxico.org.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banco-de-mexico/refs/heads/main/security/banco-de-mexico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Central Bank
- Mexico
- Economic Data
- Payments
---
