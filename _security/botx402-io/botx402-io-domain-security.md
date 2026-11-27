---
api_specs:
- filename: botx402-io-agent-api-openapi.yml
  format: yaml
  label: BotX402 Agent API
  slug: botx402-io-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botx402-io/openapi/botx402-io-agent-api-openapi.yml
- filename: botx402-io-base-address-balance-api-openapi.yml
  format: yaml
  label: BotX402 Base Address Balance API
  slug: botx402-io-base-address-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botx402-io/openapi/botx402-io-base-address-balance-api-openapi.yml
- filename: botx402-io-well-known-api-openapi.yml
  format: yaml
  label: BotX402 .well Known API
  slug: botx402-io-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botx402-io/openapi/botx402-io-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botx402.io
  spf: true
hosts:
- cert_expires: Apr 27 23:59:59 2027 GMT
  host: botx402.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BotX402 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BotX402, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BotX402
provider_slug: botx402-io
slug: botx402-io-domain-security
source_filename: botx402-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botx402.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: botx402.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/botx402-io/security/botx402-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pay-per-use
- Bots
- Business
- Automation
- SaaS-alternative
---
