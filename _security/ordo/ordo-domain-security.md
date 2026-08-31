---
api_specs:
- filename: ordo-account-data-client-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Data - Client Hosted API
  slug: ordo-account-data-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-client-hosted-api-openapi.yml
- filename: ordo-account-data-ordo-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Data - Ordo Hosted API
  slug: ordo-account-data-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-ordo-hosted-api-openapi.yml
- filename: ordo-account-verification-client-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Verification - Client Hosted API
  slug: ordo-account-verification-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-verification-client-hosted-api-openapi.yml
- filename: ordo-account-verification-ordo-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Verification - Ordo Hosted API
  slug: ordo-account-verification-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-verification-ordo-hosted-api-openapi.yml
- filename: ordo-bank-accounts-api-openapi.yml
  format: yaml
  label: Ordo Bank accounts API
  slug: ordo-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-bank-accounts-api-openapi.yml
- filename: ordo-client-hosted-api-openapi.yml
  format: yaml
  label: Ordo Client hosted API
  slug: ordo-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-client-hosted-api-openapi.yml
- filename: ordo-create-a-mandate-api-openapi.yml
  format: yaml
  label: Ordo Create a mandate API
  slug: ordo-create-a-mandate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-create-a-mandate-api-openapi.yml
- filename: ordo-ordo-hosted-api-openapi.yml
  format: yaml
  label: Ordo Ordo hosted API
  slug: ordo-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-ordo-hosted-api-openapi.yml
- filename: ordo-retrieve-mandate-details-api-openapi.yml
  format: yaml
  label: Ordo Retrieve mandate details API
  slug: ordo-retrieve-mandate-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-retrieve-mandate-details-api-openapi.yml
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
