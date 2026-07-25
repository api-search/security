---
api_specs:
- filename: peachpayments-authentication-api-openapi.yml
  format: yaml
  label: Peach Payments Authentication API
  slug: peachpayments-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-authentication-api-openapi.yml
- filename: peachpayments-checkout-api-openapi.yml
  format: yaml
  label: Peach Payments Checkout API
  slug: peachpayments-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-checkout-api-openapi.yml
- filename: peachpayments-payment-links-api-openapi.yml
  format: yaml
  label: Peach Payments Payment Links API
  slug: peachpayments-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-payment-links-api-openapi.yml
- filename: peachpayments-payments-api-openapi.yml
  format: yaml
  label: Peach Payments Payments API
  slug: peachpayments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-payments-api-openapi.yml
- filename: peachpayments-payouts-api-openapi.yml
  format: yaml
  label: Peach Payments Payouts API
  slug: peachpayments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-payouts-api-openapi.yml
- filename: peachpayments-reconciliation-api-openapi.yml
  format: yaml
  label: Peach Payments Reconciliation API
  slug: peachpayments-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-reconciliation-api-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: mailto:security@peachpayments.com
  dnssec: false
  domain: peachpayments.com
  spf: true
  spf_record: v=spf1 include:7856266.spf06.hubspotemail.net include:spf.mandrillapp.com include:_spf.google.com include:fdspfaus.freshemail.io ~all
hosts:
- cert_expires: Oct 10 19:19:52 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: www.peachpayments.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:07:24 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: developer.peachpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)
  host: dashboard.peachpayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)
  host: api-v2.peachpayments.com
  http_status: 403
  https: true
  notes: 403 on bare GET; expected for OAuth/entityId-gated POST payment endpoint.
- cert_expires: Dec 10 23:59:59 2026 GMT
  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)
  host: payouts.peachpayments.com
  http_status: 403
  https: true
  notes: 403 on bare GET; expected for Bearer-gated payout endpoint.
- cert_expires: Dec 10 23:59:59 2026 GMT
  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)
  host: secure.peachpayments.com
  http_status: 403
  https: true
  notes: 403 on bare GET; expected for Bearer/entityId-gated Checkout endpoint.
kind: domain-security
layout: security
method: probed
name: Peachpayments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peach Payments, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peach Payments
provider_slug: peachpayments
slug: peachpayments-domain-security
source_filename: peachpayments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peachpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Oct 10 19:19:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n- host: developer.peachpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  3 22:07:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.peachpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: api-v2.peachpayments.com\n  https: true\n  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  http_status: 403\n  notes: 403 on bare GET; expected for OAuth/entityId-gated POST payment\
  \ endpoint.\n- host: payouts.peachpayments.com\n  https: true\n  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  http_status: 403\n  notes: 403 on bare GET; expected for Bearer-gated payout endpoint.\n- host: secure.peachpayments.com\n  https: true\n  cert_issuer: Sectigo Limited (Public Server Authentication CA DV R36)\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  http_status: 403\n  notes: 403 on bare GET; expected for Bearer/entityId-gated Checkout endpoint.\ndomains:\n- domain: peachpayments.com\n  dnssec: false\n  spf: true\n  spf_record: v=spf1 include:7856266.spf06.hubspotemail.net include:spf.mandrillapp.com include:_spf.google.com include:fdspfaus.freshemail.io ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: mailto:security@peachpayments.com\ncompliance:\n- PCI DSS Level 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/security/peachpayments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Africa
- Payment Gateway
- Checkout
- Payouts
---
