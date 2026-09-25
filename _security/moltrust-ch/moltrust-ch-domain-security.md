---
api_specs:
- filename: moltrust-ch-openapi.yml
  format: yaml
  label: MolTrust API
  slug: moltrust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moltrust-ch/refs/heads/main/openapi/moltrust-ch-openapi.yml
- filename: moltrust-ch-moltguard-openapi.yml
  format: yaml
  label: MoltGuard API
  slug: moltguard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moltrust-ch/refs/heads/main/openapi/moltrust-ch-moltguard-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moltrust.ch
  spf: true
hosts:
- cert_expires: Nov 15 12:13:48 2026 GMT
  host: moltrust.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 12:13:48 2026 GMT
  host: api.moltrust.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 11:50:37 2026 GMT
  host: uresolver.moltrust.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Moltrust Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MolTrust, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MolTrust
provider_slug: moltrust-ch
slug: moltrust-ch-domain-security
source_filename: moltrust-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moltrust.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 12:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moltrust.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 12:13:48 2026 GMT\n  hsts: null\n- host: uresolver.moltrust.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 11:50:37 2026 GMT\n  hsts: null\ndomains:\n- domain: moltrust.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moltrust-ch/refs/heads/main/security/moltrust-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Agent Identity
- Decentralized Identity
- Verifiable Credentials
- Trust and Safety
- Agent Authorization
- Compliance
- Blockchain
- A2A
- MCP
- x402
- Agent-Native
---
