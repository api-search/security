---
api_specs:
- filename: superform-openapi-original.json
  format: json
  label: Superform API
  slug: superform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: superform.xyz
  spf: true
hosts:
- cert_expires: Oct 11 17:47:35 2026 GMT
  host: superform.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 09:00:03 2026 GMT
  host: api.superform.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superform, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Superform
provider_slug: superform
slug: superform-domain-security
source_filename: superform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superform.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:47:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.superform.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:00:03 2026 GMT\n  hsts: null\ndomains:\n- domain: superform.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/security/superform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi Yield
- DeFi
- Vaults
- Yield Aggregation
- Cross Chain
- Onchain
- Blockchain
- Smart Accounts
---
