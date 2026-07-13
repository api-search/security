---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lovable.dev
  spf: true
hosts:
- cert_expires: Sep  2 20:24:30 2026 GMT
  host: lovable.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 20:54:34 2026 GMT
  host: docs.lovable.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 08:46:57 2026 GMT
  host: mcp.lovable.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lovable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lovable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lovable
provider_slug: lovable
slug: lovable-domain-security
source_filename: lovable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovable.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:24:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lovable.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:54:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.lovable.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:46:57 2026 GMT\n  hsts: false\ndomains:\n- domain: lovable.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovable/refs/heads/main/security/lovable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- No-Code
- App Builder
- Web Development
- Generative
- MCP
---
