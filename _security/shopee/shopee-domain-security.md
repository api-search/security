---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopee.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopeemobile.com
  spf: true
hosts:
- cert_expires: Sep 27 10:05:16 2026 GMT
  host: open.shopee.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 12:08:12 2026 GMT
  host: partner.shopeemobile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopee, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shopee
provider_slug: shopee
slug: shopee-domain-security
source_filename: shopee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.shopee.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 10:05:16 2026 GMT\n  hsts: false\n- host: partner.shopeemobile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 12:08:12 2026 GMT\n  hsts: null\ndomains:\n- domain: shopee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: shopeemobile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopee/refs/heads/main/security/shopee-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- E-commerce
- Marketplace
- Southeast Asia
- Cross-border
- Orders
- Products
- Logistics
- Shopee
---
