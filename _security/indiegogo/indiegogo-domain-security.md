---
api_specs:
- filename: indiegogo-public-openapi.yml
  format: yaml
  label: Indiegogo Public API
  slug: indiegogo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indiegogo/refs/heads/main/openapi/indiegogo-public-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: indiegogo.com
  spf: true
hosts:
- cert_expires: Sep  7 20:59:37 2026 GMT
  host: indiegogo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indiegogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indiegogo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Indiegogo
provider_slug: indiegogo
slug: indiegogo-domain-security
source_filename: indiegogo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indiegogo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:59:37 2026 GMT\n  hsts: null\ndomains:\n- domain: indiegogo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indiegogo/refs/heads/main/security/indiegogo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Crowdfunding
- Fundraising
- Campaigns
- Payments
- Marketplace
- Creators
---
