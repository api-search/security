---
api_specs:
- filename: unlock-site-content-api-openapi.yml
  format: yaml
  label: Unlock Site Content API
  slug: unlock-site-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-site-content-api-openapi.yml
- filename: unlock-editorial-api-openapi.yml
  format: yaml
  label: Unlock Editorial API
  slug: unlock-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-editorial-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unlock.com
  spf: true
hosts:
- cert_expires: Nov  6 14:11:58 2026 GMT
  host: www.unlock.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unlock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unlock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unlock
provider_slug: unlock
slug: unlock-domain-security
source_filename: unlock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unlock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:11:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: unlock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/security/unlock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- FinTech
- Home Equity
- Mortgage
- Real Estate
- Consumer Lending
- Home Equity Agreement
- Personal Finance
- Content
---
