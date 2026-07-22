---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paireyewear.com
  spf: true
hosts:
- cert_expires: Sep  3 19:11:03 2026 GMT
  host: paireyewear.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pair Eyewear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pair Eyewear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pair Eyewear
provider_slug: pair-eyewear
slug: pair-eyewear-domain-security
source_filename: pair-eyewear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paireyewear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: paireyewear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pair-eyewear/refs/heads/main/security/pair-eyewear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Eyewear
- Ecommerce
- Retail
- Shopify
- Direct-to-Consumer
- Agent Commerce
- MCP
- UCP
---
