---
api_specs:
- filename: curlec-razorpay-openapi.json
  format: json
  label: Razorpay Curlec REST API
  slug: razorpay-curlec-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curlec/refs/heads/main/openapi/curlec-razorpay-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curlec.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: razorpay.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: curlec.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.razorpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curlec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curlec, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Curlec
provider_slug: curlec
slug: curlec-domain-security
source_filename: curlec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curlec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: api.razorpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: curlec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: razorpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curlec/refs/heads/main/security/curlec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Gateway
- Recurring Payments
- Subscriptions
- Direct Debit
- FinTech
- Malaysia
- DuitNow
- FPX
- Webhooks
- Razorpay
---
