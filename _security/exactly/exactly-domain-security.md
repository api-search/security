---
api_specs:
- filename: previewer-api.yml
  format: yaml
  label: Exactly Protocol Previewer API
  slug: exactly-protocol-previewer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/previewer-api.yml
- filename: market-api.yml
  format: yaml
  label: Exactly Protocol Market API
  slug: exactly-protocol-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/market-api.yml
- filename: auditor-api.yml
  format: yaml
  label: Exactly Protocol Auditor API
  slug: exactly-protocol-auditor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/auditor-api.yml
- filename: rewards-controller-api.yml
  format: yaml
  label: Exactly Protocol RewardsController API
  slug: exactly-protocol-rewardscontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/rewards-controller-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exact.ly
  spf: true
hosts:
- cert_expires: Sep 13 16:43:41 2026 GMT
  host: exact.ly
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 22:03:36 2026 GMT
  host: docs.exact.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 12:09:16 2026 GMT
  host: app.exact.ly
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exactly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exactly Protocol, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Exactly Protocol
provider_slug: exactly
slug: exactly-domain-security
source_filename: exactly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exact.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.exact.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.exact.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 12:09:16 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: exact.ly\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/security/exactly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- Lending
- Borrowing
- Fixed Rate
- Variable Rate
- Ethereum
- Optimism
- Base
- ERC-4626
- Credit Markets
---
