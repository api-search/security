---
api_specs:
- filename: api-guide
  format: yaml
  label: Toss Payments API
  slug: toss-payments-api
  spec_type: OpenAPI
  url: https://docs.tosspayments.com/en/api-guide
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: toss.im
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tosspayments.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: toss.im
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: docs.tosspayments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.tosspayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toss, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Toss
provider_slug: toss
slug: toss-domain-security
source_filename: toss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toss.im\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: docs.tosspayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: api.tosspayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: toss.im\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tosspayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toss/refs/heads/main/security/toss-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Payments
- Fintech
- Banking
- Korea
- Digital Wallet
- Credit Scoring
- Identity Verification
- Financial Services
- Super App
---
