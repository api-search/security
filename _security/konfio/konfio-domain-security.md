---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konfio.mx
  spf: true
hosts:
- cert_expires: Aug 14 19:41:43 2026 GMT
  host: konfio.mx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Konfio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konfio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Konfio
provider_slug: konfio
slug: konfio-domain-security
source_filename: konfio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konfio.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:41:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: konfio.mx\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konfio/refs/heads/main/security/konfio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SMB Lending
- Business Banking
- Credit Cards
- Payment Terminals
- Fintech
- Mexico
- Latin America
---
