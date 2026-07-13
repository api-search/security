---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: connectrpc.com
  spf: false
hosts:
- cert_expires: Oct  2 15:05:40 2026 GMT
  host: connectrpc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connect Rpc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connect-RPC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Connect-RPC
provider_slug: connect-rpc
slug: connect-rpc-domain-security
source_filename: connect-rpc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connectrpc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:05:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: connectrpc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connect-rpc/refs/heads/main/security/connect-rpc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Apache 2.0
- Buf
- Code Generation
- Connect Protocol
- gRPC
- gRPC-Web
- HTTP
- Open Source
- Protocol Buffers
- RPC
- SDKs
---
