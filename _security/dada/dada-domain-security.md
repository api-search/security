---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imdada.cn
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: imdada.cn
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dada
provider_slug: dada
slug: dada-domain-security
source_filename: dada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imdada.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: imdada.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dada/refs/heads/main/security/dada-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Delivery
- Logistics
- Instant Retail
- Last-Mile Delivery
- On-Demand
- Local Commerce
- China
- JD
---
