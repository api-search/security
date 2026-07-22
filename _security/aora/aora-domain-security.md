---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: aoraservicios.com
  spf: true
hosts:
- cert_expires: Aug 30 05:28:57 2026 GMT
  host: aoraservicios.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Aora
provider_slug: aora
slug: aora-domain-security
source_filename: aora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aoraservicios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 05:28:57 2026 GMT\n  hsts: false\ndomains:\n- domain: aoraservicios.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aora/refs/heads/main/security/aora-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Home Services
- On-Demand
- Marketplace
- Mexico
- Field Services
- Appliances
- Consumer
---
