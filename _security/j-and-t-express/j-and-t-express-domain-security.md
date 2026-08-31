---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jtexpress.com
  spf: true
hosts:
- cert_expires: Oct 24 02:19:47 2026 GMT
  host: jtexpress.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: J And T Express Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for J&T Express, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: J&T Express
provider_slug: j-and-t-express
slug: j-and-t-express-domain-security
source_filename: j-and-t-express-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jtexpress.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 02:19:47 2026 GMT\n  hsts: false\ndomains:\n- domain: jtexpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/j-and-t-express/refs/heads/main/security/j-and-t-express-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Consumer
- Logistics
- Delivery
- Shipping
- Express
- Supply Chain
- E-Commerce
- Courier
- Track and Trace
---
