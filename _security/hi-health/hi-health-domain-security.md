---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getpliant.com
  spf: true
hosts:
- cert_expires: Aug 25 10:31:41 2026 GMT
  host: customer-api.getpliant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: partner-api.getpliant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hi Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hi Health
provider_slug: hi-health
slug: hi-health-domain-security
source_filename: hi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: customer-api.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:31:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-api.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getpliant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hi-health/refs/heads/main/security/hi-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Insurance
- Payments
- Fintech
- Card Issuing
- Reimbursement
- InsurTech
- Digital Health
- Speedinvest
---
