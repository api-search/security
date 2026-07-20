---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gigstack.pro
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gigstack.io
  spf: true
hosts:
- cert_expires: Sep 13 16:47:05 2026 GMT
  host: gigstack.pro
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 00:03:58 2026 GMT
  host: docs.gigstack.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 13:57:32 2026 GMT
  host: api.gigstack.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gigstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gigstack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gigstack
provider_slug: gigstack
slug: gigstack-domain-security
source_filename: gigstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigstack.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:47:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: docs.gigstack.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  3 00:03:58 2026 GMT\n  hsts: false\n- host: api.gigstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:57:32 2026 GMT\n  hsts: null\ndomains:\n- domain: gigstack.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gigstack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigstack/refs/heads/main/security/gigstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Invoicing
- CFDI
- SAT
- Tax Compliance
- Payments
- Billing
- Collections
- Mexico
- Accounts Receivable
---
