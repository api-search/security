---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uship.com
  spf: true
hosts:
- cert_expires: Sep 16 10:16:24 2026 GMT
  host: www.uship.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 17:05:25 2026 GMT
  host: developer.uship.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 16 10:16:24 2026 GMT
  host: api.uship.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for uShip, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: uShip
provider_slug: uship
slug: uship-domain-security
source_filename: uship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.uship.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 17:05:25 2026 GMT\n  hsts: false\n- host: api.uship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:16:24 2026 GMT\n  hsts: null\ndomains:\n- domain: uship.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uship/refs/heads/main/security/uship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Shipping
- Logistics
- freight
- Marketplace
- Transportation
- auto-transport
- ltl-freight
- last-mile-delivery
- shipment-tracking
- E-Commerce
- Supply Chain
- rate-quotes
---
