---
api_specs:
- filename: ledger-investing-analytics-openapi.yml
  format: yaml
  label: Ledger Analytics API
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger-investing/refs/heads/main/openapi/ledger-investing-analytics-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ledgerinvesting.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: readthedocs-hosted.com
  spf: false
hosts:
- cert_expires: Sep 20 20:20:08 2026 GMT
  host: www.ledgerinvesting.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 18:43:48 2026 GMT
  host: ledger-investing-ledger-analytics.readthedocs-hosted.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:29:14 2026 GMT
  host: api.korra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ledger Investing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ledger Investing, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ledger Investing
provider_slug: ledger-investing
slug: ledger-investing-domain-security
source_filename: ledger-investing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ledgerinvesting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:20:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ledger-investing-ledger-analytics.readthedocs-hosted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.korra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:29:14 2026 GMT\n  hsts: null\ndomains:\n- domain: ledgerinvesting.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readthedocs-hosted.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledger-investing/refs/heads/main/security/ledger-investing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance Tech
- Insurance
- Reinsurance
- Insurance-Linked Securities
- Actuarial
- Analytics
- Capital Markets
- Data Science
- Financial Services
---
