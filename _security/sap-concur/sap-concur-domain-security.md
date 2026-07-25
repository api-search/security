---
api_specs:
- filename: sap-concur-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Allocations API
  slug: sap-concur-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/openapi/sap-concur-allocations-api-openapi.yml
- filename: sap-concur-comments-api-openapi.yml
  format: yaml
  label: SAP Concur Comments API
  slug: sap-concur-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/openapi/sap-concur-comments-api-openapi.yml
- filename: sap-concur-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expenses API
  slug: sap-concur-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/openapi/sap-concur-expenses-api-openapi.yml
- filename: sap-concur-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Reports API
  slug: sap-concur-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/openapi/sap-concur-reports-api-openapi.yml
- filename: sap-concur-workflows-api-openapi.yml
  format: yaml
  label: SAP Concur Workflows API
  slug: sap-concur-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/openapi/sap-concur-workflows-api-openapi.yml
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
