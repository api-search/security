---
api_specs:
- filename: xflow-openapi-original.yml
  format: yaml
  label: Xflow API
  slug: xflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/openapi/xflow-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xflowpay.com
  spf: true
hosts:
- cert_expires: Sep 15 08:46:01 2026 GMT
  host: www.xflowpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: dashboard.xflowpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: docs.xflowpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xflow
provider_slug: xflow
slug: xflow-domain-security
source_filename: xflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xflowpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:46:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dashboard.xflowpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.xflowpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xflowpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xflow/refs/heads/main/security/xflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Cross-Border Payments
- Fintech
- India
- Foreign Exchange
- Invoicing
- Payouts
---
