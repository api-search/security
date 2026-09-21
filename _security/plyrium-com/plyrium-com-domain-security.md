---
api_specs:
- filename: plyrium-com-vouchspec-openapi.yml
  format: yaml
  label: VouchSpec Agent Skill Evidence API
  slug: vouchspec-agent-skill-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plyrium-com/refs/heads/main/openapi/plyrium-com-vouchspec-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plyrium.com
  spf: true
hosts:
- cert_expires: Nov 26 18:33:49 2026 GMT
  host: plyrium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 18:33:49 2026 GMT
  host: www.plyrium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 18:33:49 2026 GMT
  host: vouchspec.plyrium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Plyrium Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plyrium, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Plyrium
provider_slug: plyrium-com
slug: plyrium-com-domain-security
source_filename: plyrium-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plyrium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 18:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.plyrium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 18:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: vouchspec.plyrium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 18:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: plyrium.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plyrium-com/refs/heads/main/security/plyrium-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agent Skills
- Supply Chain Security
- Software Provenance
- x402
- Agentic Commerce
- A2A
- MCP
- Field Service
- Home Services
---
