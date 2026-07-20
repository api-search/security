---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firework.com
  spf: true
hosts:
- cert_expires: Sep  3 09:58:40 2026 GMT
  host: docs.firework.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.firework.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firework, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Firework
provider_slug: firework
slug: firework-domain-security
source_filename: firework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.firework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:58:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.firework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: firework.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firework/refs/heads/main/security/firework-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Video Commerce
- Shoppable Video
- Livestream Shopping
- Ecommerce
- Retail
- Video
- SDK
- Webhooks
---
