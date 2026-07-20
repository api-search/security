---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deppon.com
  spf: true
hosts:
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: www.deppon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: dpopen.deppon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deppon Express Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deppon Express, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Deppon Express
provider_slug: deppon-express
slug: deppon-express-domain-security
source_filename: deppon-express-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deppon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: false\n- host: dpopen.deppon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: deppon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deppon-express/refs/heads/main/security/deppon-express-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Logistics
- Express Delivery
- Shipping
- Freight
- Supply Chain
- Tracking
- E-commerce
- China
---
