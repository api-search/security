---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloomandwild.com
  spf: true
hosts:
- cert_expires: Oct 10 12:48:10 2026 GMT
  host: www.bloomandwild.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloom And Wild Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloom & Wild, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bloom & Wild
provider_slug: bloom-and-wild
slug: bloom-and-wild-domain-security
source_filename: bloom-and-wild-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomandwild.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 12:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: bloomandwild.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloom-and-wild/refs/heads/main/security/bloom-and-wild-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Flowers
- Gifting
- E-Commerce
- Subscription
- Delivery
- Retail
---
