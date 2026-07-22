---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kaminashi.jp
  spf: false
hosts:
- cert_expires: Oct  5 18:55:19 2026 GMT
  host: kaminashi.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ulysses Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ulysses (Kaminashi), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ulysses (Kaminashi)
provider_slug: ulysses
slug: ulysses-domain-security
source_filename: ulysses-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaminashi.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:55:19 2026 GMT\n  hsts: false\ndomains:\n- domain: kaminashi.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ulysses/refs/heads/main/security/ulysses-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- SaaS
- Frontline Operations
- Manufacturing
- Food Safety
- CMMS
- Training
- Deskless Workforce
- Japan
---
