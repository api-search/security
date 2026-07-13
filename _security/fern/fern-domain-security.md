---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buildwithfern.com
  spf: false
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: buildwithfern.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Fern
provider_slug: fern
slug: fern-domain-security
source_filename: fern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildwithfern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildwithfern.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fern/refs/heads/main/security/fern-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Ready
- AI
- API Definitions
- AsyncAPI
- Code Generation
- Developer Experience
- Developer Portal
- Documentation
- gRPC
- llms.txt
- MCP
- OpenAPI
- OpenRPC
- Platform
- Protobuf
- SDKs
- WebSockets
---
