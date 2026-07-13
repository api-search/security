---
api_specs:
- filename: index.html
  format: yaml
  label: CyberSource Payments API
  slug: cybersource-payments-api
  spec_type: OpenAPI
  url: https://developer.cybersource.com/api-reference-assets/index.html
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@visa.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cybersource.com
  spf: true
hosts:
- cert_expires: Oct 18 21:35:02 2026 GMT
  host: developer.cybersource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.cybersource.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: apitest.cybersource.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cybersource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyberSource, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CyberSource
provider_slug: cybersource
slug: cybersource-domain-security
source_filename: cybersource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cybersource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 21:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cybersource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: apitest.cybersource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cybersource.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hostmaster@visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybersource/refs/heads/main/security/cybersource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Fraud Management
- Tokenization
- Recurring Billing
- Payouts
- Payment Gateway
- Financial Technology
---
