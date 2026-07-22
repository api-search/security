---
api_specs:
- filename: loon-finance-transparency-openapi.yml
  format: yaml
  label: Loon CADC Transparency API
  slug: loon-cadc-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loon-finance/refs/heads/main/openapi/loon-finance-transparency-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loon.finance
  spf: false
hosts:
- cert_expires: Aug 24 17:59:47 2026 GMT
  host: loon.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loon Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loon Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Loon Finance
provider_slug: loon-finance
slug: loon-finance-domain-security
source_filename: loon-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loon.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:59:47 2026 GMT\n  hsts: false\ndomains:\n- domain: loon.finance\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loon-finance/refs/heads/main/security/loon-finance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Stablecoin
- Cryptocurrency
- Payments
- Canada
- Digital Dollar
- Blockchain
- Transparency
---
