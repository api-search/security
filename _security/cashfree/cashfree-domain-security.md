---
api_specs:
- filename: openapi-payment-gateway.json
  format: json
  label: Cashfree Payment Gateway API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/openapi/openapi-payment-gateway.json
- filename: openapi-payouts.json
  format: json
  label: Cashfree Payouts API
  slug: payouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/openapi/openapi-payouts.json
- filename: openapi-verification.json
  format: json
  label: Cashfree Secure ID (Verification) API
  slug: secure-id
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/openapi/openapi-verification.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cashfree.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.cashfree.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.cashfree.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: payout-api.cashfree.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cashfree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cashfree Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cashfree Payments
provider_slug: cashfree
slug: cashfree-domain-security
source_filename: cashfree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cashfree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.cashfree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\n- host: payout-api.cashfree.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cashfree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashfree/refs/heads/main/security/cashfree-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payouts
- UPI
- India
- Payment Gateway
- Subscriptions
- Refunds
- QR Codes
- Net Banking
- Identity Verification
---
