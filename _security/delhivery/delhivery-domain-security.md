---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: delhivery.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.delhivery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delhivery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delhivery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Delhivery
provider_slug: delhivery
slug: delhivery-domain-security
source_filename: delhivery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.delhivery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: delhivery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delhivery/refs/heads/main/security/delhivery-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Shipping
- Supply Chain
- Freight
- Ecommerce
- Tracking
- Fulfillment
- India
---
