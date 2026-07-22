---
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@vestwell.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vestwell.com
  spf: true
hosts:
- cert_expires: Sep 20 21:13:49 2026 GMT
  host: www.vestwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vestwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vestwell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vestwell
provider_slug: vestwell
slug: vestwell-domain-security
source_filename: vestwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vestwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vestwell.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:admin@vestwell.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vestwell/refs/heads/main/security/vestwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retirement
- Workplace Savings
- 401(k)
- 529 College Savings
- Financial Services
- Fintech
- Recordkeeping
- Payroll Integration
- State Retirement Programs
---
