---
api_specs:
- filename: gl-api.json
  format: json
  label: Oracle General Ledger API
  slug: oracle-general-ledger-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/openapi/gl-api.json
- filename: ap-api.json
  format: json
  label: Oracle Accounts Payable API
  slug: oracle-accounts-payable-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/openapi/ap-api.json
- filename: ar-api.json
  format: json
  label: Oracle Accounts Receivable API
  slug: oracle-accounts-receivable-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/openapi/ar-api.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: support.oracle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Financials 12 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Financials 12, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Financials 12
provider_slug: oracle-financials-12
slug: oracle-financials-12-domain-security
source_filename: oracle-financials-12-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: support.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financials-12/refs/heads/main/security/oracle-financials-12-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- E-Business Suite
- Enterprise
- ERP
- Financial Management
- Oracle
- Release 12
---
