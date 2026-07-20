---
api_specs:
- filename: finix-payments-openapi-original.yml
  format: yaml
  label: Finix API
  slug: finix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix-payments/refs/heads/main/openapi/finix-payments-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finixpayments.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: sandbox-payments-api.com
  spf: false
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.finixpayments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: finix.sandbox-payments-api.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Finix Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finix Payments, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Finix Payments
provider_slug: finix-payments
slug: finix-payments-domain-security
source_filename: finix-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finixpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n- host: finix.sandbox-payments-api.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finixpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sandbox-payments-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finix-payments/refs/heads/main/security/finix-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Processing
- Payment Facilitation
- Embedded Finance
- Marketplaces
- ACH
- Card Acceptance
- Fintech
- PCI DSS
---
