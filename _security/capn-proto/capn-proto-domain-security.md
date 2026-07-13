---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: capnproto.org
  spf: true
hosts:
- cert_expires: Aug 25 13:49:09 2026 GMT
  host: capnproto.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capn Proto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cap''n Proto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cap'n Proto
provider_slug: capn-proto
slug: capn-proto-domain-security
source_filename: capn-proto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capnproto.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capnproto.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capn-proto/refs/heads/main/security/capn-proto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Binary Format
- Capability-Based Security
- Code Generation
- IPC
- Open Source
- Protocol
- RPC
- Schema
- SDKs
- Serialization
- Specification
- Zero Copy
---
