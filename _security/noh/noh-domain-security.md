---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: noh.com.br
  spf: true
hosts:
- cert_expires: Sep  1 03:13:17 2026 GMT
  host: noh.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Noh
provider_slug: noh
slug: noh-domain-security
source_filename: noh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noh.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noh.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noh/refs/heads/main/security/noh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Neobank
- Payments
- Banking
- Consumer Finance
- Brazil
- Couples
---
