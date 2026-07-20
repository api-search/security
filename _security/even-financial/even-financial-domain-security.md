---
api_specs:
- filename: even-financial-openapi-original.json
  format: json
  label: Engine by MoneyLion API
  slug: engine-by-moneylion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/even-financial/refs/heads/main/openapi/even-financial-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: engine.tech
  spf: true
hosts:
- cert_expires: Sep 14 06:24:38 2026 GMT
  host: api.engine.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Even Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Even Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Even Financial
provider_slug: even-financial
slug: even-financial-domain-security
source_filename: even-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.engine.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:24:38 2026 GMT\n  hsts: null\ndomains:\n- domain: engine.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/even-financial/refs/heads/main/security/even-financial-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Embedded Finance
- Fintech
- Lending
- Personal Loans
- Credit Cards
- Marketplace
- Recommendation Engine
- Lead Generation
---
