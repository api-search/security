---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lalamove.com
  spf: true
hosts:
- cert_expires: Oct 29 12:29:58 2026 GMT
  host: lalamove.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 12:29:58 2026 GMT
  host: developers.lalamove.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 12:29:58 2026 GMT
  host: rest.lalamove.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lalamove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lalamove, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lalamove
provider_slug: lalamove
slug: lalamove-domain-security
source_filename: lalamove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lalamove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 12:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.lalamove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 12:29:58 2026 GMT\n  hsts: false\n- host: rest.lalamove.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 12:29:58 2026 GMT\n  hsts: null\ndomains:\n- domain: lalamove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lalamove/refs/heads/main/security/lalamove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technology
- Logistics
- Delivery
- Last Mile Delivery
- Courier
- Transportation
- On Demand
- Fleet
- Shipping
---
