---
api_specs:
- filename: mintmcp-openapi-generated.yml
  format: yaml
  label: MintMCP API
  slug: mintmcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mintmcp/refs/heads/main/openapi/_ae-authored/mintmcp-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mintmcp.com
  spf: true
hosts:
- cert_expires: Dec 26 16:40:56 2026 GMT
  host: mintmcp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mintmcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MintMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MintMCP
provider_slug: mintmcp
slug: mintmcp-domain-security
source_filename: mintmcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mintmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:40:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mintmcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mintmcp/refs/heads/main/security/mintmcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Platform
- Enterprise
- Security
- Integration
---
