---
api_specs:
- filename: blocktorch-hardhat-forking-openapi.yml
  format: yaml
  label: Blocktorch Hardhat Forking API
  slug: blocktorch-hardhat-forking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blocktorch/refs/heads/main/openapi/blocktorch-hardhat-forking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blocktorch.xyz
  spf: true
hosts:
- host: blocktorch.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Blocktorch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blocktorch, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Blocktorch
provider_slug: blocktorch
slug: blocktorch-domain-security
source_filename: blocktorch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blocktorch.xyz\n  https: false\ndomains:\n- domain: blocktorch.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blocktorch/refs/heads/main/security/blocktorch-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Web3
- Observability
- Monitoring
- Blockchain
- Smart Contracts
- dApps
- Developer Tools
---
