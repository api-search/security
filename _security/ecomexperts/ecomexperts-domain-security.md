---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ecomexperts.com
  spf: true
hosts:
- cert_expires: Sep  8 11:34:28 2026 GMT
  host: ecomexperts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ecomexperts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcomExperts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EcomExperts
provider_slug: ecomexperts
slug: ecomexperts-domain-security
source_filename: ecomexperts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecomexperts.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 11:34:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ecomexperts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecomexperts/refs/heads/main/security/ecomexperts-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Ecommerce
- ERP
- Omnichannel
- Inventory Management
- Electronic Invoicing
- Marketplace Integration
- Mercado Libre
- SaaS
- Latin America
---
