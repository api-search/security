---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: recruitee.com
  spf: true
hosts:
- cert_expires: Sep  4 14:47:49 2026 GMT
  host: recruitee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:59:10 2026 GMT
  host: docs.recruitee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recruitee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recruitee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Recruitee
provider_slug: recruitee
slug: recruitee-domain-security
source_filename: recruitee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recruitee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:47:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.recruitee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: recruitee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/security/recruitee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recruiting
- ATS
- Applicant Tracking
- HR
- Hiring
- Careers Site
- Tellent
---
