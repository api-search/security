---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Bamboo Investment API
  slug: bamboo-investment-api
  spec_type: OpenAPI
  url: https://docs.investbamboo.com/api/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: investbamboo.com
  spf: true
hosts:
- cert_expires: Oct  4 15:15:46 2026 GMT
  host: investbamboo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:15:46 2026 GMT
  host: docs.investbamboo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:15:46 2026 GMT
  host: api.investbamboo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bamboo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bamboo Invest, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bamboo Invest
provider_slug: bamboo
slug: bamboo-domain-security
source_filename: bamboo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: investbamboo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:15:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.investbamboo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:15:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.investbamboo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:15:46 2026 GMT\n  hsts: null\ndomains:\n- domain: investbamboo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bamboo/refs/heads/main/security/bamboo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Investments
- Stocks
- Fractional Shares
- Africa
- Nigeria
- Portfolio Management
- Brokerage
- Fintech
---
