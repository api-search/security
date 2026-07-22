---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: epsor.fr
  spf: true
hosts:
- cert_expires: Sep  9 14:14:44 2026 GMT
  host: www.epsor.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epsor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epsor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Epsor
provider_slug: epsor
slug: epsor-domain-security
source_filename: epsor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epsor.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epsor.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsor/refs/heads/main/security/epsor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Employee Savings
- Retirement
- Épargne Salariale
- HR
- Compensation and Benefits
- ESG
- France
---
