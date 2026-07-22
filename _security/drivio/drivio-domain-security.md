---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: drivio.in
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: www.drivio.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Drivio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drivio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Drivio
provider_slug: drivio
slug: drivio-domain-security
source_filename: drivio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drivio.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drivio.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drivio/refs/heads/main/security/drivio-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Financial Services
- Lending
- Fintech
- Two-Wheeler Financing
- Loans
- EMI
- India
- Marketplace
- Electric Vehicles
---
