---
api_specs:
- filename: ordo-single-payments.yml
  format: yaml
  label: Ordo Single Payments API
  slug: ordo-single-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-single-payments.yml
- filename: ordo-smart-request-manager.yml
  format: yaml
  label: Ordo Smart Request Manager API
  slug: ordo-smart-request-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-smart-request-manager.yml
- filename: ordo-recurring-payment-mandates.yml
  format: yaml
  label: Ordo Recurring Payment Mandates (VRP) API
  slug: ordo-recurring-payment-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-recurring-payment-mandates.yml
- filename: ordo-account-data-ordo-hosted.yml
  format: yaml
  label: Ordo Account Data (Ordo Hosted) API
  slug: ordo-account-data-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-ordo-hosted.yml
- filename: ordo-account-data-client-hosted.yml
  format: yaml
  label: Ordo Account Data (Client Hosted) API
  slug: ordo-account-data-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-client-hosted.yml
- filename: ordo-registry-manager.yml
  format: yaml
  label: Ordo Registry Manager API
  slug: ordo-registry-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-registry-manager.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ordopay.com
  spf: true
hosts:
- cert_expires: Sep 10 06:53:57 2026 GMT
  host: ordopay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: test.api.ordopay.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ordo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ordo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ordo
provider_slug: ordo
slug: ordo-domain-security
source_filename: ordo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ordopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:53:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: test.api.ordopay.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ordopay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/security/ordo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Open Banking
- Account-to-Account
- Payment Initiation
- Variable Recurring Payments
- Request to Pay
- Real-Time Payments
- Faster Payments
- PSD2
- Account Information
---
