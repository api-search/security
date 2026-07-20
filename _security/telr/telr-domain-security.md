---
api_specs:
- filename: telr-openapi.yml
  format: yaml
  label: Telr Hosted Payment Page API
  slug: telr-hosted-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Remote API
  slug: telr-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Digital Wallets API
  slug: telr-digital-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Repeat Billing API
  slug: telr-repeat-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Payments REST API
  slug: telr-payments-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Mobile API and SDKs
  slug: telr-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
description: ''
domains:
- domain: telr.com
  note: No /.well-known/security.txt published at telr.com as of the probe date.
  security_txt: false
  security_txt_status: 404
hosts:
- cert_expires: Sep  4 07:01:06 2026 GMT
  cert_not_before: Jun  6 06:01:18 2026 GMT
  host: telr.com
  http_status: 200
  https: true
  tls_issuer: Google Trust Services (WE1)
- cert_expires: Sep 22 04:27:27 2026 GMT
  cert_not_before: Jun 24 03:27:34 2026 GMT
  host: secure.telr.com
  http_status: 405
  https: true
  note: Payment gateway host; 405 on GET / (POST-only JSON endpoints under /gateway and /api/v1). GET /gateway/order.json returned 200.
  tls_issuer: Google Trust Services (WE1)
- cert_expires: Oct 14 20:41:14 2026 GMT
  cert_not_before: Jul 16 20:41:15 2026 GMT
  host: docs.telr.com
  http_status: 302
  https: true
  tls_issuer: Let's Encrypt (YE2)
kind: domain-security
layout: security
method: probed
name: Telr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Telr
provider_slug: telr
slug: telr-domain-security
source_filename: telr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + docs hosts (2026-07-17)\nhosts:\n- host: telr.com\n  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_not_before: Jun  6 06:01:18 2026 GMT\n  cert_expires: Sep  4 07:01:06 2026 GMT\n  http_status: 200\n- host: secure.telr.com\n  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_not_before: Jun 24 03:27:34 2026 GMT\n  cert_expires: Sep 22 04:27:27 2026 GMT\n  http_status: 405\n  note: Payment gateway host; 405 on GET / (POST-only JSON endpoints under /gateway and /api/v1). GET /gateway/order.json returned 200.\n- host: docs.telr.com\n  https: true\n  tls_issuer: Let's Encrypt (YE2)\n  cert_not_before: Jul 16 20:41:15 2026 GMT\n  cert_expires: Oct 14 20:41:14 2026 GMT\n  http_status: 302\ndomains:\n- domain: telr.com\n  security_txt: false\n  security_txt_status: 404\n  note: No /.well-known/security.txt published at telr.com as of the probe date.\ncompliance:\n\
  - PCI DSS v4.0 Level 1\n- NESA certified (first PCI-DSS Level 1 & NESA-certified company in MENA)\n- Central Bank of the UAE Retail Payment Services (RPS) license\n- 3-D Secure (payer authentication) supported on hosted and remote flows\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/security/telr-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Payments
- Payment Gateway
- FinTech
- MENA
- UAE
---
