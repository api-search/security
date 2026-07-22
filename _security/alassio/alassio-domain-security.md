---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alassio.fr
  spf: true
hosts:
- cert_expires: Aug 28 12:05:49 2026 GMT
  host: www.alassio.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alassio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alassio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Alassio
provider_slug: alassio
slug: alassio-domain-security
source_filename: alassio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alassio.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:05:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alassio.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alassio/refs/heads/main/security/alassio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Financial Services
- Payroll
- Human Resources
- HR Tech
- Payroll Software
- SaaS
- France
- Fintech
- Compensation
---
