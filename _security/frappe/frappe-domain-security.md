---
api_specs:
- filename: frappe-method-api-openapi.yml
  format: yaml
  label: Frappe Method API
  slug: frappe-method-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frappe/refs/heads/main/openapi/frappe-method-api-openapi.yml
- filename: frappe-resource-api-openapi.yml
  format: yaml
  label: Frappe Resource API
  slug: frappe-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frappe/refs/heads/main/openapi/frappe-resource-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: frappe.io
  spf: true
hosts:
- cert_expires: Sep 22 11:43:54 2026 GMT
  host: frappe.io
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
kind: domain-security
layout: security
method: probed
name: Frappe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frappe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Frappe
provider_slug: frappe
slug: frappe-domain-security
source_filename: frappe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frappe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.frappe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: frappe.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frappe/refs/heads/main/security/frappe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Source
- ERP
- Accounting
- Inventory
- Payroll
- Low Code
---
