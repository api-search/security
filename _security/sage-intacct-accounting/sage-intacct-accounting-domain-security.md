---
api_specs:
- filename: intacct-openapi
  format: yaml
  label: Sage Intacct REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://developer.sage.com/intacct/apis/intacct/1/intacct-openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: intacct.com
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: www.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:04:19 2026 GMT
  host: developer.sage.com
  hsts: true
  hsts_max_age: 15552000
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
name: Sage Intacct Accounting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sage Intacct Accounting, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sage Intacct Accounting
provider_slug: sage-intacct-accounting
slug: sage-intacct-accounting-domain-security
source_filename: sage-intacct-accounting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.intacct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:46:40 2026 GMT\n  hsts: null\ndomains:\n- domain: sage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: intacct.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage-intacct-accounting/refs/heads/main/security/sage-intacct-accounting-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Financial Management
- ERP
- Cloud Accounting
- General Ledger
- Accounts Payable
- Accounts Receivable
- Revenue Recognition
- Multi-Entity
---
