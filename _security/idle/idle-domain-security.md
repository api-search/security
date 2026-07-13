---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Idle Finance API
  slug: idle-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idle/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: idle.finance
  spf: true
hosts:
- cert_expires: Sep 27 16:33:26 2026 GMT
  host: idle.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:11:14 2026 GMT
  host: docs.idle.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.idle.finance
  https: false
kind: domain-security
layout: security
method: probed
name: Idle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Idle Finance, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Idle Finance
provider_slug: idle
slug: idle-domain-security
source_filename: idle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: idle.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:33:26 2026 GMT\n  hsts: false\n- host: docs.idle.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.idle.finance\n  https: false\ndomains:\n- domain: idle.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idle/refs/heads/main/security/idle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Yield Optimization
- Finance
- Crypto
- Staking
- Governance
- TVL
- APY
---
