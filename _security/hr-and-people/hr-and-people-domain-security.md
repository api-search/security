---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bamboohr.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: services1.workday.com
  https: false
- cert_expires: Oct  3 02:39:04 2026 GMT
  host: documentation.bamboohr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hr And People Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HR & People, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HR & People
provider_slug: hr-and-people
slug: hr-and-people-domain-security
source_filename: hr-and-people-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: services1.workday.com\n  https: false\n- host: documentation.bamboohr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:39:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bamboohr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hr-and-people/refs/heads/main/security/hr-and-people-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- People Operations
- Payroll
- Talent Acquisition
- Performance Management
- Employee Engagement
- People Data
- Workforce Management
- Unified API
---
