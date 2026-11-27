---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: employeedeskhq.com
  spf: true
hosts:
- cert_expires: Jan 24 20:39:04 2027 GMT
  host: employeedeskhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EmployeeDeskHQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmployeeDeskHQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EmployeeDeskHQ
provider_slug: employeedeskhq-com
slug: employeedeskhq-com-domain-security
source_filename: employeedeskhq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: employeedeskhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 20:39:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: employeedeskhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/employeedeskhq-com/security/employeedeskhq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Communications
- Software-as-a-Service
- Employee Engagement
- Productivity
- Small Business
---
