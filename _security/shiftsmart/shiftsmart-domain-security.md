---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shiftsmart.com
  spf: true
hosts:
- cert_expires: Oct 15 11:24:03 2026 GMT
  host: shiftsmart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:17:25 2026 GMT
  host: api.shiftsmart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shiftsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shiftsmart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shiftsmart
provider_slug: shiftsmart
slug: shiftsmart-domain-security
source_filename: shiftsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shiftsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:24:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shiftsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:17:25 2026 GMT\n  hsts: null\ndomains:\n- domain: shiftsmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiftsmart/refs/heads/main/security/shiftsmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Management
- Staffing
- Scheduling
- Labor Marketplace
- Human Resources
- Gig Economy
- Workforce
- Payments
- Field Services
---
