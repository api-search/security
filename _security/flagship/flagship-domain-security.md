---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flagship.shop
  spf: true
hosts:
- cert_expires: Oct 16 00:02:12 2026 GMT
  host: landing.flagship.shop
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flagship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flagship, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flagship
provider_slug: flagship
slug: flagship-domain-security
source_filename: flagship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landing.flagship.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:02:12 2026 GMT\n  hsts: null\ndomains:\n- domain: flagship.shop\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagship/refs/heads/main/security/flagship-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- E-commerce
- Shopping
- Consumer
- Startup
---
