---
api_specs:
- filename: ontopx402-bidding-api-openapi.yml
  format: yaml
  label: OnTopX402 Bidding API
  slug: ontopx402-bidding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontopx402/refs/heads/main/openapi/ontopx402-bidding-api-openapi.yml
- filename: ontopx402-leaderboard-api-openapi.yml
  format: yaml
  label: OnTopX402 Leaderboard API
  slug: ontopx402-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontopx402/refs/heads/main/openapi/ontopx402-leaderboard-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ontopx402.com
  spf: true
hosts:
- cert_expires: Nov 19 02:30:28 2026 GMT
  host: ontopx402.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ontopx402 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OnTopX402, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OnTopX402
provider_slug: ontopx402
slug: ontopx402-domain-security
source_filename: ontopx402-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ontopx402.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 02:30:28 2026 GMT\n  hsts: null\ndomains:\n- domain: ontopx402.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontopx402/refs/heads/main/security/ontopx402-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- x402
- USDC
- Agent Payments
- paid-placement
- Leaderboard
---
