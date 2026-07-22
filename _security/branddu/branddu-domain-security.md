---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: branddu.com
  spf: true
hosts:
- cert_expires: Sep  4 02:44:33 2026 GMT
  host: branddu.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Branddu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branddu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Branddu
provider_slug: branddu
slug: branddu-domain-security
source_filename: branddu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branddu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:44:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: branddu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branddu/refs/heads/main/security/branddu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Merchandising
- Promotional Products
- Procurement
- MerchTech
- E-Commerce
- B2B
- Shopify
- Colombia
---
