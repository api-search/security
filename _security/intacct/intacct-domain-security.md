---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sageintacct.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.com
  spf: true
hosts:
- cert_expires: Aug 21 16:47:30 2026 GMT
  host: www.sageintacct.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:04:19 2026 GMT
  host: developer.sage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:46:40 2026 GMT
  host: api.intacct.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intacct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sage Intacct, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Sage Intacct
provider_slug: intacct
slug: intacct-domain-security
source_filename: intacct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sageintacct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:47:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:04:19 2026 GMT\n  hsts: null\n- host: api.intacct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:46:40 2026 GMT\n  hsts: null\ndomains:\n- domain: sageintacct.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intacct/refs/heads/main/security/intacct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounting
- ERP
- Financial Management
- Cloud Accounting
- Invoicing
- Payments
- SaaS
- REST API
- OAuth
---
