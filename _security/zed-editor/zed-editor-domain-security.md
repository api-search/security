---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zed.dev
  spf: true
hosts:
- cert_expires: Oct  7 20:01:03 2026 GMT
  host: zed.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zed Editor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zed
provider_slug: zed-editor
slug: zed-editor-domain-security
source_filename: zed-editor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zed.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:01:03 2026 GMT\n  hsts: false\ndomains:\n- domain: zed.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zed-editor/refs/heads/main/security/zed-editor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Code Editor
- Developer Tools
- IDE
- Rust
- GPU Accelerated
- Open Source
- AI Coding
- Agentic Editing
- Real-Time Collaboration
- Language Server Protocol
- Debug Adapter Protocol
- Model Context Protocol
- Agent Client Protocol
- WebAssembly Extensions
- Tree-sitter
- Multiplayer
---
