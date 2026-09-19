---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: insperity.com
  spf: true
hosts:
- cert_expires: Nov 24 14:08:01 2026 GMT
  host: www.insperity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 15:50:49 2026 GMT
  host: developer.insperity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  7 13:02:21 2026 GMT
  host: api.insperity.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Insperity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insperity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Insperity
provider_slug: insperity
slug: insperity-domain-security
source_filename: insperity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insperity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 14:08:01 2026 GMT\n  hsts: null\n- host: developer.insperity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 15:50:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.insperity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 13:02:21 2026 GMT\n  hsts: null\ndomains:\n- domain: insperity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insperity/refs/heads/main/security/insperity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
- Human Resources
- Payroll
- Benefits
- HRIS
- Onboarding
- Professional Employer Organization
- Workforce Management
- Employer of Record
---
