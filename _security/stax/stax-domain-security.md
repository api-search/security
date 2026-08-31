---
api_specs:
- filename: stax-api-openapi.json
  format: json
  label: Stax API
  slug: stax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/openapi/stax-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: staxpayments.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fattlabs.com
  spf: false
hosts:
- cert_expires: Oct 13 03:31:46 2026 GMT
  host: staxpayments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 01:47:13 2026 GMT
  host: docs.staxpayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: apiprod.fattlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stax, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stax
provider_slug: stax
slug: stax-domain-security
source_filename: stax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: staxpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 03:31:46 2026 GMT\n  hsts: false\n- host: docs.staxpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 01:47:13 2026 GMT\n  hsts: null\n- host: apiprod.fattlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: staxpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fattlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/security/stax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payment Processing
- Merchant Services
- Embedded Payments
- ACH
- Invoicing
- Subscription Billing
- Surcharging
- Point of Sale
- Tokenization
- Financial Services
- Fintech
- Card Present
- Merchant Onboarding
---
