---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mottu.com.br
  spf: true
hosts:
- cert_expires: Oct 11 18:25:24 2026 GMT
  host: mottu.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mottu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mottu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mottu
provider_slug: mottu
slug: mottu-domain-security
source_filename: mottu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mottu.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:25:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mottu.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mottu/refs/heads/main/security/mottu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Mobility
- Motorcycle Rental
- Last-Mile Delivery
- Logistics
- Brazil
- Latin America
- Gig Economy
---
