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
- cert_expires: Sep 18 14:37:43 2026 GMT
  host: www.getpliant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:54:36 2026 GMT
  host: partner.getpliant.com
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
name: Hihealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hi.health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: hi.health
provider_slug: hihealth
slug: hihealth-domain-security
source_filename: hihealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:37:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:54:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-api.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getpliant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hihealth/refs/heads/main/security/hihealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Payments
- Cards
- Fintech
- Health
- Cards-as-a-Service
- Embedded Finance
- Reimbursement
- Claims
---
