---
api_specs:
- filename: grounded-tools-docs-mcp-server-openapi.yml
  format: yaml
  label: Grounded.tools
  slug: grounded-tools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grounded-tools/refs/heads/main/openapi/grounded-tools-docs-mcp-server-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: grounded.tools
  spf: true
hosts:
- cert_expires: Oct  1 18:02:01 2026 GMT
  host: grounded.tools
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grounded Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grounded.tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Grounded.tools
provider_slug: grounded-tools
slug: grounded-tools-domain-security
source_filename: grounded-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grounded.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grounded.tools\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grounded-tools/refs/heads/main/security/grounded-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Developer Tools
- Developers
- Documentation
- Experience
---
