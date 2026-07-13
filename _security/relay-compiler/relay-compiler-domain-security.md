---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: relay.dev
  spf: true
hosts:
- cert_expires: Aug 24 05:01:58 2026 GMT
  host: relay.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relay Compiler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relay Compiler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Relay Compiler
provider_slug: relay-compiler
slug: relay-compiler-domain-security
source_filename: relay-compiler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relay.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:01:58 2026 GMT\n  hsts: false\ndomains:\n- domain: relay.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relay-compiler/refs/heads/main/security/relay-compiler-domain-security.yml
summary_line: TLSv1.3
tags:
- Code Generation
- GraphQL
- React
- Meta
- Open Source
- TypeScript
- Build Tools
---
