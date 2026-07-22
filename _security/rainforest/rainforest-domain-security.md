---
api_specs:
- filename: rainforest-payments-openapi.yaml
  format: yaml
  label: Rainforest Payments API
  slug: rainforest-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest/refs/heads/main/openapi/rainforest-payments-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rainforestpay.com
  spf: true
hosts:
- cert_expires: Sep 11 03:33:26 2026 GMT
  host: www.rainforestpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.sandbox.rainforestpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.rainforestpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rainforest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainforest, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rainforest
provider_slug: rainforest
slug: rainforest-domain-security
source_filename: rainforest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rainforestpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:33:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sandbox.rainforestpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\n- host: api.rainforestpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: rainforestpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainforest/refs/heads/main/security/rainforest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Embedded Payments
- Payment Facilitator
- Payment Processing
- Vertical SaaS
- Fintech
- ACH
---
