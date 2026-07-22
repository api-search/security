---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: monakapp.com
  spf: true
hosts:
- cert_expires: Sep 10 16:13:56 2026 GMT
  host: monakapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monak E Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monak E-Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Monak E-Services
provider_slug: monak-e-services
slug: monak-e-services-domain-security
source_filename: monak-e-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monakapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:13:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monakapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monak-e-services/refs/heads/main/security/monak-e-services-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Banking
- Remittance
- Payments
- Super App
- Middle East
- Expat Services
---
