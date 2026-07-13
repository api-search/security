---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rappi.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.rappi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: dev-portal.rappi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rappi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rappi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rappi
provider_slug: rappi
slug: rappi-domain-security
source_filename: rappi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rappi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\n- host: dev-portal.rappi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rappi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rappi/refs/heads/main/security/rappi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Delivery
- Food Delivery
- Grocery Delivery
- On-Demand
- Last Mile
- Logistics
- Super App
- Fintech
- Payments
- Marketplace
- Latin America
- Colombia
---
