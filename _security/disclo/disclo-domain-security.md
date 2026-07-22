---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: disclo.com
  spf: true
hosts:
- cert_expires: Sep 10 09:07:28 2026 GMT
  host: www.disclo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disclo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Disclo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Disclo
provider_slug: disclo
slug: disclo-domain-security
source_filename: disclo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.disclo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:07:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: disclo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disclo/refs/heads/main/security/disclo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workplace Accommodations
- Disability
- HR Tech
- ADA Compliance
- FMLA
- Leave Management
- Medical Certification
- HRIS Integration
- Health Data
---
