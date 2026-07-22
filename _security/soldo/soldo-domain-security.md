---
api_specs:
- filename: soldo-business-api-v20-openapi-original.json
  format: json
  label: Soldo Business API v2.0
  slug: soldo-business-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soldo/refs/heads/main/openapi/soldo-business-api-v20-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soldo.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: soldocloud.net
  spf: false
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.soldo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.soldo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api-demo.soldocloud.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Soldo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soldo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Soldo
provider_slug: soldo
slug: soldo-domain-security
source_filename: soldo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soldo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.soldo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: api-demo.soldocloud.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: soldo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: soldocloud.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soldo/refs/heads/main/security/soldo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fintech
- Financial Services
- Spend Management
- Expense Management
- Business Cards
- Prepaid Cards
- Payments
- Banking
---
