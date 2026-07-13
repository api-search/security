---
api_specs:
- filename: sage-accounting-openapi.yml
  format: yaml
  label: Sage Accounting API
  slug: accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-accounting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.com
  spf: true
hosts:
- cert_expires: Sep 29 04:04:19 2026 GMT
  host: developer.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: www.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.accounting.sage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sage
provider_slug: sage
slug: sage-domain-security
source_filename: sage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.accounting.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/security/sage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Business Management
- Cloud Software
- ERP
- Payroll
- HR
---
