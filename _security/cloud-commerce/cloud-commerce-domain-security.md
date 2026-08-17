---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudcommerce.co
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fastship.co
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: cloudcommerce.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: fastship.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: openapi.fastship.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cloud Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Commerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cloud Commerce
provider_slug: cloud-commerce
slug: cloud-commerce-domain-security
source_filename: cloud-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudcommerce.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: fastship.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: openapi.fastship.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cloudcommerce.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: fastship.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-commerce/refs/heads/main/security/cloud-commerce-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Logistics
- Marketplace
- Influencer Marketing
- Cross-Border Commerce
- SME
- Southeast Asia
- Shipping
- Fulfillment
- Thailand
---
