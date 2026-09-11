---
api_specs:
- filename: aelf-inc-node-web-api-openapi.json
  format: json
  label: aelf Node Web API
  slug: aelf-node-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aelf-inc/refs/heads/main/openapi/aelf-inc-node-web-api-openapi.json
- filename: aelf-inc-agent-gateway-openapi.yaml
  format: yaml
  label: aelf Agent Gateway API
  slug: aelf-agent-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aelf-inc/refs/heads/main/openapi/aelf-inc-agent-gateway-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aelf.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aelf.io
  spf: true
hosts:
- cert_expires: Oct 12 15:56:00 2026 GMT
  host: aelf.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 15:56:00 2026 GMT
  host: docs.aelf.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 17:43:11 2026 GMT
  host: aelf-public-node.aelf.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aelf Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aelf, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aelf
provider_slug: aelf-inc
slug: aelf-inc-domain-security
source_filename: aelf-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aelf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:56:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.aelf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:56:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: aelf-public-node.aelf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 17:43:11 2026 GMT\n  hsts: null\ndomains:\n- domain: aelf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aelf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aelf-inc/refs/heads/main/security/aelf-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Layer 1
- Web3
- Smart Contracts
- Cross-Chain
- Developer Tools
- Protobuf
- Agent Skills
- Cryptocurrency
---
