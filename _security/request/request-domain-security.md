---
api_specs:
- filename: 24913360-b5105a65-a6bd-4247-b3b1-ed60e5c8f5cb
  format: yaml
  label: Request Finance AP and AR API
  slug: request-finance-ap-and-ar-api
  spec_type: Postman
  url: https://www.postman.com/request-finance/workspace/request-finance-api-public/documentation/24913360-b5105a65-a6bd-4247-b3b1-ed60e5c8f5cb
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: request.finance
  spf: true
hosts:
- cert_expires: Sep 26 07:06:19 2026 GMT
  host: www.request.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 02:25:47 2026 GMT
  host: docs.request.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 08:02:16 2026 GMT
  host: api.request.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Request Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Request Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Request Finance
provider_slug: request
slug: request-domain-security
source_filename: request-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.request.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:06:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.request.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 02:25:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.request.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:02:16 2026 GMT\n  hsts: null\ndomains:\n- domain: request.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/request/refs/heads/main/security/request-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Invoicing
- Crypto
- Web3
- Payroll
- Stablecoins
- Accounts Payable
- Accounts Receivable
- Fintech
- Blockchain
- REST API
---
