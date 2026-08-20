---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salliemae.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.salliemae.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sallie Mae Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sallie Mae Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sallie Mae Bank
provider_slug: sallie-mae
slug: sallie-mae-domain-security
source_filename: sallie-mae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.salliemae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: salliemae.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sallie-mae/refs/heads/main/security/sallie-mae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Industrial Bank
- Student Loans
- Savings
- Consumer Finance
- Data Aggregation
---
