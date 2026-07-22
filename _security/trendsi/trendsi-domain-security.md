---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trendsi.com
  spf: true
hosts:
- cert_expires: Jan 29 12:19:51 2027 GMT
  host: trendsi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trendsi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trendsi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trendsi
provider_slug: trendsi
slug: trendsi-domain-security
source_filename: trendsi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trendsi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 12:19:51 2027 GMT\n  hsts: false\ndomains:\n- domain: trendsi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trendsi/refs/heads/main/security/trendsi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fashion
- Wholesale
- Dropshipping
- Ecommerce
- Apparel
- Shopify
- TikTok Shop
- Retail
- Fulfillment
---
