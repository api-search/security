---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: worksome.com
  spf: true
hosts:
- cert_expires: Oct 14 16:12:27 2026 GMT
  host: www.worksome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 17:20:57 2026 GMT
  host: docs.worksome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 04:18:27 2026 GMT
  host: api.worksome.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Worksome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worksome, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Worksome
provider_slug: worksome
slug: worksome-domain-security
source_filename: worksome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.worksome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:12:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.worksome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 17:20:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.worksome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 04:18:27 2026 GMT\n  hsts: null\ndomains:\n- domain: worksome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worksome/refs/heads/main/security/worksome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freelancer Management System
- Contingent Workforce
- Human Resources
- Staffing
- Workforce Compliance
- Payments
- GraphQL
- Webhooks
- Denmark
---
