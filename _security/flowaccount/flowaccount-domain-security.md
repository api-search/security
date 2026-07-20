---
api_specs:
- filename: flowaccount-openapi-original.json
  format: json
  label: FlowAccount Open API
  slug: flowaccount-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:security@flowaccount.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flowaccount.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: flowaccount.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: openapi.flowaccount.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowaccount Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlowAccount, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FlowAccount
provider_slug: flowaccount
slug: flowaccount-domain-security
source_filename: flowaccount-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowaccount.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.flowaccount.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: flowaccount.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:security@flowaccount.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/security/flowaccount-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounting
- Invoicing
- Payroll
- Point of Sale
- SME
- Finance
- Tax
- Thailand
- Bookkeeping
---
