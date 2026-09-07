---
api_specs:
- filename: zenledger-compliance-api-openapi.yml
  format: yaml
  label: ZenLedger Compliance Suite API
  slug: zenledger-compliance-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-compliance-api-openapi.yml
- filename: zenledger-aggregator-api-openapi.yml
  format: yaml
  label: ZenLedger Aggregator Suite API
  slug: zenledger-aggregator-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-aggregator-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenledger.io
  spf: true
hosts:
- cert_expires: Nov 24 20:16:20 2026 GMT
  host: zenledger.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:25:31 2026 GMT
  host: docs.zenledger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 06:11:07 2026 GMT
  host: api.zenledger.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Zenledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenLedger, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ZenLedger
provider_slug: zenledger
slug: zenledger-domain-security
source_filename: zenledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 20:16:20 2026 GMT\n  hsts: null\n- host: docs.zenledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:25:31 2026 GMT\n  hsts: false\n- host: api.zenledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 06:11:07 2026 GMT\n  hsts: null\ndomains:\n- domain: zenledger.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/security/zenledger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Crypto Tax
- Digital Assets
- Tax Compliance
- Blockchain Analytics
- RegTech
- Accounting
- Sanctions Screening
- Financial Services
- Portfolio Aggregation
- Cryptocurrency
---
