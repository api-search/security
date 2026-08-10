---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: allworknow.com
  spf: true
hosts:
- cert_expires: Oct 30 15:34:35 2026 GMT
  host: allworknow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: app.allworknow.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: application host (CloudFront)
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: auth.allworknow.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Keycloak identity provider, realm AWN1
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AllWork, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AllWork
provider_slug: allwork
slug: allwork-domain-security
source_filename: allwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allworknow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 15:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.allworknow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  note: application host (CloudFront)\n- host: auth.allworknow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Keycloak identity provider, realm AWN1\ndomains:\n- domain: allworknow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allwork/refs/heads/main/security/allwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Workforce Management
- Human Resources
- Staffing
- Payroll
- Employer of Record
- Contingent Workforce
- Gig Economy
- Scheduling
- Time and Attendance
- Compliance
---
