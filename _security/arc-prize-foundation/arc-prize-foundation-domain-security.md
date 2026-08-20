---
api_specs:
- filename: arc-prize-foundation-commands-api-openapi.yml
  format: yaml
  label: Arc Prize Foundation Commands API
  slug: arc-prize-foundation-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arc-prize-foundation/refs/heads/main/openapi/arc-prize-foundation-commands-api-openapi.yml
- filename: arc-prize-foundation-games-api-openapi.yml
  format: yaml
  label: Arc Prize Foundation Games API
  slug: arc-prize-foundation-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arc-prize-foundation/refs/heads/main/openapi/arc-prize-foundation-games-api-openapi.yml
- filename: arc-prize-foundation-scorecards-api-openapi.yml
  format: yaml
  label: Arc Prize Foundation Scorecards API
  slug: arc-prize-foundation-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arc-prize-foundation/refs/heads/main/openapi/arc-prize-foundation-scorecards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arcprize.org
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: three.arcprize.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Arc Prize Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arc Prize Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arc Prize Foundation
provider_slug: arc-prize-foundation
slug: arc-prize-foundation-domain-security
source_filename: arc-prize-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: three.arcprize.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: arcprize.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arc-prize-foundation/refs/heads/main/security/arc-prize-foundation-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- AGI
- Benchmarks
- Agents
- Reasoning
- Machine-Learning
- Non-Profit
---
