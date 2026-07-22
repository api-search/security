---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: queroquitar.com.br
  spf: true
hosts:
- cert_expires: Oct 15 21:23:29 2026 GMT
  host: queroquitar.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Queroquitar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QueroQuitar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QueroQuitar
provider_slug: queroquitar
slug: queroquitar-domain-security
source_filename: queroquitar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: queroquitar.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:23:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: queroquitar.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queroquitar/refs/heads/main/security/queroquitar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Debt Negotiation
- Debt Settlement
- Financial Services
- Consumer Finance
- Brazil
---
