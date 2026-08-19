---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: powder.gg
  spf: true
hosts:
- cert_expires: Nov  5 23:06:43 2026 GMT
  host: powder.gg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Powder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Powder
provider_slug: powder
slug: powder-domain-security
source_filename: powder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powder.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powder.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powder/refs/heads/main/security/powder-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Video
- Artificial Intelligence
- Content Creation
- Streaming
- Media
- Desktop Application
- Discontinued
---
