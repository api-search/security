---
api_specs:
- filename: aza-finance-openapi-original.json
  format: json
  label: TransferZero API V1
  slug: transferzero-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azafinance.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transferzero.com
  spf: true
hosts:
- cert_expires: Oct  9 03:37:43 2026 GMT
  host: www.azafinance.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:46:24 2026 GMT
  host: api-sandbox.transferzero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:46:24 2026 GMT
  host: api.transferzero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aza Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AZA Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AZA Finance
provider_slug: aza-finance
slug: aza-finance-domain-security
source_filename: aza-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.azafinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:37:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api-sandbox.transferzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:46:24 2026 GMT\n  hsts: null\n- host: api.transferzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:46:24 2026 GMT\n  hsts: null\ndomains:\n- domain: azafinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: transferzero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/security/aza-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Payments
- Foreign Exchange
- Cross-Border Payments
- Africa
- Fintech
- API
---
