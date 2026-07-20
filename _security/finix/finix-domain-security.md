---
api_specs:
- filename: finix-openapi-original.yml
  format: yaml
  label: Finix API
  slug: finix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: live-payments-api.com
  spf: false
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: finix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 00:59:36 2026 GMT
  host: docs.finix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: finix.live-payments-api.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Finix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Finix
provider_slug: finix
slug: finix-domain-security
source_filename: finix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: docs.finix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:59:36 2026 GMT\n  hsts: false\n- host: finix.live-payments-api.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: live-payments-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/security/finix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Payment Processing
- Payment Facilitation
- Merchant Onboarding
- Payouts
- Marketplaces
---
