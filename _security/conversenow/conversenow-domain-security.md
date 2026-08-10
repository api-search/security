---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: conversenow.ai
  spf: true
hosts:
- cert_expires: Oct  2 07:40:53 2026 GMT
  host: conversenow.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conversenow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConverseNow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ConverseNow
provider_slug: conversenow
slug: conversenow-domain-security
source_filename: conversenow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conversenow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:40:53 2026 GMT\n  hsts: false\ndomains:\n- domain: conversenow.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conversenow/refs/heads/main/security/conversenow-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Voice AI
- Conversational AI
- Restaurants
- Point of Sale
- Ordering
- Drive-Thru
- Speech Recognition
- Artificial Intelligence
- Food Service
---
