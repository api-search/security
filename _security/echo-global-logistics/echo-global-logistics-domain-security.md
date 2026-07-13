---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: echo.com
  spf: true
hosts:
- cert_expires: Oct  5 09:28:03 2026 GMT
  host: www.echo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Echo Global Logistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echo Global Logistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Echo Global Logistics
provider_slug: echo-global-logistics
slug: echo-global-logistics-domain-security
source_filename: echo-global-logistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.echo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 09:28:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: echo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo-global-logistics/refs/heads/main/security/echo-global-logistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Freight
- Trucking
- Supply Chain
- Third Party Logistics
- Freight Brokerage
- LTL
- Truckload
- Intermodal
- EDI
- Transportation Management
- B2B
---
