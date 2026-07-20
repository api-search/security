---
api_specs:
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Payment Requests API
  slug: hitpay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Recurring Billing API
  slug: hitpay-recurring-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Subscription Plans API
  slug: hitpay-subscription-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Refunds API
  slug: hitpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Platform API
  slug: hitpay-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
description: ''
domains:
- caa: []
  dnssec: false
  domain: hitpayapp.com
  note: No CAA records returned on probe.
- caa: []
  dnssec: false
  domain: hit-pay.com
  note: No CAA records returned on probe. API served from api.hit-pay.com.
hosts:
- cert_expires: Sep 24 10:31:35 2026 GMT
  cert_issuer: Let's Encrypt
  host: www.hitpayapp.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 10:38:35 2027 GMT
  cert_issuer: GoDaddy Secure Certificate Authority - G2
  host: api.hit-pay.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  hsts_preload: true
  https: true
  note: Root path returns 404; API base is /v1 and requires X-BUSINESS-API-KEY.
  tls_version: TLSv1.3
- cert_expires: Sep 24 10:31:35 2026 GMT
  cert_issuer: Let's Encrypt
  host: docs.hitpayapp.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hitpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HitPay, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HitPay
provider_slug: hitpay
slug: hitpay-domain-security
source_filename: hitpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hitpayapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 24 10:31:35 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: api.hit-pay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GoDaddy Secure Certificate Authority - G2\n  cert_expires: Jan 21 10:38:35 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Root path returns 404; API base is /v1 and requires X-BUSINESS-API-KEY.\n- host: docs.hitpayapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 24 10:31:35 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: hitpayapp.com\n  dnssec: false\n  caa: []\n  note: No\
  \ CAA records returned on probe.\n- domain: hit-pay.com\n  dnssec: false\n  caa: []\n  note: No CAA records returned on probe. API served from api.hit-pay.com.\nsecurityTxt:\n  present: false\n  note: No /.well-known/security.txt served (request 308-redirects without a file).\ncompliance:\n  pci_dss: true\n  note: >-\n    HitPay is PCI DSS compliant and is a regulated payment institution; it holds\n    a Major Payment Institution (MPI) posture with the Monetary Authority of\n    Singapore (MAS) and is regulated across multiple APAC jurisdictions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/security/hitpay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Payments
- Fintech
- PayNow
- Southeast Asia
- SMB
---
