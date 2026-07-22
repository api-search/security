---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: palmhr.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: palm.hr
  spf: true
hosts:
- cert_expires: Oct 10 13:53:02 2026 GMT
  host: palmhr.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 04:03:53 2026 GMT
  host: api.palm.hr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Palmhr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palm HR, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Palm HR
provider_slug: palmhr
slug: palmhr-domain-security
source_filename: palmhr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palmhr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 13:53:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.palm.hr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: palmhr.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: palm.hr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palmhr/refs/heads/main/security/palmhr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HR
- Human Resources
- Payroll
- Attendance
- Performance Management
- Recruiting
- WPS
- UAE
- MENA
---
