---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kcaldata.com
  spf: false
hosts:
- cert_expires: Dec 20 07:48:39 2026 GMT
  host: kcaldata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: kcaldata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kcaldata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: kcaldata
provider_slug: kcaldata-com
slug: kcaldata-com-domain-security
source_filename: kcaldata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kcaldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 07:48:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kcaldata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kcaldata-com/security/kcaldata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Nutrition API
- Calorie Data
- Machine‑Readable API
- Agentic Payments
- USDC
---
