---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tailcall.run
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forgecode.dev
  spf: true
hosts:
- cert_expires: Aug 21 03:37:55 2026 GMT
  host: tailcall.run
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 21:50:18 2026 GMT
  host: forgecode.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tailcall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailcall, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tailcall
provider_slug: tailcall
slug: tailcall-domain-security
source_filename: tailcall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tailcall.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:37:55 2026 GMT\n  hsts: false\n- host: forgecode.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 21:50:18 2026 GMT\n  hsts: false\ndomains:\n- domain: tailcall.run\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: forgecode.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailcall/refs/heads/main/security/tailcall-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- GraphQL
- API Gateway
- GraphQL Runtime
- REST
- gRPC
- Rust
- Open Source
- API Composition
- Caching
- Batching
---
