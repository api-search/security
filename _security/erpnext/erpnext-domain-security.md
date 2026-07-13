---
api_specs:
- filename: frappe_api-docs
  format: yaml
  label: ERPNext REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/alyf-de/frappe_api-docs
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: erpnext.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: frappe.io
  spf: true
hosts:
- cert_expires: Aug 25 16:33:42 2026 GMT
  host: erpnext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:43:54 2026 GMT
  host: docs.frappe.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 15:32:48 2026 GMT
  host: demo.erpnext.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erpnext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ERPNext, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ERPNext
provider_slug: erpnext
slug: erpnext-domain-security
source_filename: erpnext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erpnext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.frappe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.erpnext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 15:32:48 2026 GMT\n  hsts: null\ndomains:\n- domain: erpnext.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: frappe.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erpnext/refs/heads/main/security/erpnext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ERP
- Enterprise Resource Planning
- Accounting
- Inventory
- Manufacturing
- Sales
- CRM
- HR
- Open Source
---
