---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: bond.tech
  spf: true
hosts:
- cert_expires: Oct  9 10:56:42 2026 GMT
  host: docs.bond.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:33:13 2026 GMT
  host: api.bond.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bond Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bond, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bond
provider_slug: bond
slug: bond-domain-security
source_filename: bond-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bond.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bond.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:33:13 2026 GMT\n  hsts: null\ndomains:\n- domain: bond.tech\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/security/bond-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Banking as a Service
- Embedded Finance
- Fintech
- Payments
- Card Issuing
- Deposit Accounts
- Money Movement
- ACH
- KYC
- KYB
- Credit
---
