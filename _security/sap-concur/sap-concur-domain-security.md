---
api_specs:
- filename: expense-report.json
  format: json
  label: Concur Expense API
  slug: concur-expense-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/expense/expense-report/expense-report.json
- filename: itinerary.json
  format: json
  label: Concur Travel API
  slug: concur-travel-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/travel/itinerary/itinerary.json
- filename: v3.invoice.json
  format: json
  label: Concur Invoice API
  slug: concur-invoice-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/invoice/v3.invoice.json
- filename: v4.request.json
  format: json
  label: Concur Request API
  slug: concur-request-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/request/v4.request.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: concur.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: concursolutions.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: developer.concur.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.concursolutions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: us.api.concursolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Concur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Concur, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SAP Concur
provider_slug: sap-concur
slug: sap-concur-domain-security
source_filename: sap-concur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.concur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: www.concursolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.api.concursolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: concur.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: concursolutions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/security/sap-concur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
---
