---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: false
  dnssec: true
  domain: molg.ai
  spf: false
hosts:
- cert_expires: Sep 30 15:51:29 2026 GMT
  host: molg.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Molg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOLG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: MOLG
provider_slug: molg
slug: molg-domain-security
source_filename: molg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: molg.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:51:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: molg.ai\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/molg/refs/heads/main/security/molg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Circular Manufacturing
- E-Waste
- Robotics
- Recycling
- Sustainability
- Traceability
- Hardware
---
