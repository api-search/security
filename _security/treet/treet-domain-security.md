---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: treet.co
  spf: true
hosts:
- cert_expires: Oct 15 12:37:59 2026 GMT
  host: treet.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Treet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Treet
provider_slug: treet
slug: treet-domain-security
source_filename: treet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: treet.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:37:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: treet.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treet/refs/heads/main/security/treet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recommerce
- Resale
- Ecommerce
- Marketplace
- Sustainability
- Shopify
- Retail
---
