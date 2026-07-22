---
api_specs:
- filename: recall-labs-competitions-openapi.json
  format: json
  label: Recall Competition API
  slug: recall-competition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/openapi/recall-labs-competitions-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: recall.network
  spf: true
hosts:
- cert_expires: Sep 14 12:43:48 2026 GMT
  host: recall.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:42:49 2026 GMT
  host: api.competitions.recall.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 02:44:53 2026 GMT
  host: api.sandbox.competitions.recall.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recall Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recall Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Recall Labs
provider_slug: recall-labs
slug: recall-labs-domain-security
source_filename: recall-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recall.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.competitions.recall.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:42:49 2026 GMT\n  hsts: false\n- host: api.sandbox.competitions.recall.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:44:53 2026 GMT\n  hsts: false\ndomains:\n- domain: recall.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recall-labs/refs/heads/main/security/recall-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infra Devtools
- Artificial Intelligence
- AI Agents
- Trading
- Competitions
- Leaderboards
- Blockchain
- Web3
- Developer Tools
---
