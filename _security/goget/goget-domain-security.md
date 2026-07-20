---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goget.my
  spf: true
hosts:
- cert_expires: Oct  3 03:43:45 2026 GMT
  host: goget.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoGet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GoGet
provider_slug: goget
slug: goget-domain-security
source_filename: goget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goget.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goget.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goget/refs/heads/main/security/goget-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Delivery
- Logistics
- On-Demand
- Gig Economy
- Workforce
- Dispatch
- Malaysia
- Webhooks
---
