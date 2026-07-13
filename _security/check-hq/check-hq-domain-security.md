---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: checkhq.com
  spf: true
hosts:
- cert_expires: Aug 16 20:13:41 2026 GMT
  host: www.checkhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: console.checkhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 23 12:17:29 2026 GMT
  host: docs.checkhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Check Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Check, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Check
provider_slug: check-hq
slug: check-hq-domain-security
source_filename: check-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.checkhq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.checkhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:17:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: checkhq.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/check-hq/refs/heads/main/security/check-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payroll
- Embedded Payroll
- Payroll Infrastructure
- Payroll API
- Tax Filing
- Tax Calculation
- Money Movement
- HR
- Human Resources
- Workforce Management
- Fintech
- Compensation
- Benefits
- 1099
- W-2
- Contractor Payments
- Embedded Finance
---
