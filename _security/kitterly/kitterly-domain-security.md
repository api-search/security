---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cottoncuts.com
  spf: true
hosts:
- cert_expires: Oct 15 22:40:19 2026 GMT
  host: cottoncuts.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitterly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kitterly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kitterly
provider_slug: kitterly
slug: kitterly-domain-security
source_filename: kitterly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cottoncuts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:40:19 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: cottoncuts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitterly/refs/heads/main/security/kitterly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Subscriptions
- Consumer
- Crafts
- Textiles
- Direct to Consumer
---
