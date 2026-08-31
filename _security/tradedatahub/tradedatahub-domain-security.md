---
api_specs:
- filename: openapi.json
  format: json
  label: TradeDataHub Public API
  slug: tradedatahub-public-api
  spec_type: OpenAPI
  url: https://www.tradedatahub.net/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tradedatahub.net
  spf: true
hosts:
- cert_expires: Nov 19 11:44:26 2026 GMT
  host: www.tradedatahub.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradedatahub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TradeDataHub Public API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TradeDataHub Public API
provider_slug: tradedatahub
slug: tradedatahub-domain-security
source_filename: tradedatahub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradedatahub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 11:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tradedatahub.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradedatahub/refs/heads/main/security/tradedatahub-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- contractor data
- B2B Data
- Business Listings
- Datasets
- CSV
- Lead Generation
- Sales Intelligence
- x402
- agent-native
- llms-txt
- OpenAPI
---
