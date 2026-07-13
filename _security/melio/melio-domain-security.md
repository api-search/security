---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Melio Payments API
  slug: melio-payments-api
  spec_type: OpenAPI
  url: https://alpha-api.meliopayments.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meliopayments.com
  spf: true
hosts:
- cert_expires: Aug 20 08:56:00 2026 GMT
  host: meliopayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 13:10:42 2026 GMT
  host: api.meliopayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Melio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Melio
provider_slug: melio
slug: melio-domain-security
source_filename: melio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meliopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:56:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.meliopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:10:42 2026 GMT\n  hsts: null\ndomains:\n- domain: meliopayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melio/refs/heads/main/security/melio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B Payments
- Accounts Payable
- Accounts Receivable
- Bill Pay
- Vendor Payments
- ACH
- FinTech
- Small Business
- Embedded Finance
- Payment Processing
---
