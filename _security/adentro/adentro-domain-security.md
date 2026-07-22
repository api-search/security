---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adentro.com
  spf: true
hosts:
- cert_expires: Sep 25 09:28:23 2026 GMT
  host: adentro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adentro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adentro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adentro
provider_slug: adentro
slug: adentro-domain-security
source_filename: adentro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adentro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:28:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adentro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adentro/refs/heads/main/security/adentro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- WiFi Marketing
- Customer Intelligence
- Location Analytics
- Retail
- Marketing Attribution
- Guest WiFi
---
