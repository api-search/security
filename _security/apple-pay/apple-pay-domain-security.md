---
api_specs:
- filename: apple-pay-js-openapi.yml
  format: yaml
  label: Apple Pay JS API
  slug: apple-pay-js-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-js-openapi.yml
- filename: apple-pay-payment-token-openapi.yml
  format: yaml
  label: Apple Pay Payment Token API
  slug: apple-pay-payment-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-payment-token-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Aug 27 17:10:52 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 18:13:48 2026 GMT
  host: apple-pay-gateway.apple.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:18:09 2026 GMT
  host: apple-pay-gateway-nc-pod5.apple.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apple Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apple Pay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apple Pay
provider_slug: apple-pay
slug: apple-pay-domain-security
source_filename: apple-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apple-pay-gateway.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 18:13:48 2026 GMT\n  hsts: null\n- host: apple-pay-gateway-nc-pod5.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:18:09 2026 GMT\n  hsts: null\ndomains:\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/security/apple-pay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apple
- Contactless Payments
- Digital Wallet
- E-Commerce
- Mobile Payments
- Payments
---
