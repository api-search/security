---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greentoe.com
  spf: true
hosts:
- cert_expires: Oct 16 01:48:21 2026 GMT
  host: greentoe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greentoe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greentoe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Greentoe
provider_slug: greentoe
slug: greentoe-domain-security
source_filename: greentoe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greentoe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:48:21 2026 GMT\n  hsts: false\ndomains:\n- domain: greentoe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greentoe/refs/heads/main/security/greentoe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-commerce
- Retail
- Marketplace
- Consumer
- Electronics
- Price Negotiation
- Shopping
---
