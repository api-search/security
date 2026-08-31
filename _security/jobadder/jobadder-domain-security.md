---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jobadder.com
  spf: true
hosts:
- cert_expires: Aug 19 02:12:06 2026 GMT
  host: jobadder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 04:23:37 2026 GMT
  host: developers.jobadder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:28:07 2026 GMT
  host: api.jobadder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jobadder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JobAdder, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JobAdder
provider_slug: jobadder
slug: jobadder-domain-security
source_filename: jobadder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobadder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:12:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.jobadder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:23:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jobadder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:28:07 2026 GMT\n  hsts: null\ndomains:\n- domain: jobadder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobadder/refs/heads/main/security/jobadder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recruitment
- Applicant Tracking System
- Staffing
- Human Resources
- Talent Acquisition
- Hiring
---
