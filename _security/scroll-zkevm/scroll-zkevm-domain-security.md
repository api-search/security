---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scroll.io
  spf: true
hosts:
- cert_expires: Sep 29 04:32:01 2026 GMT
  host: scroll.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 10:39:56 2026 GMT
  host: docs.scroll.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 05:53:50 2026 GMT
  host: rpc.scroll.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scroll Zkevm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scroll, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scroll
provider_slug: scroll-zkevm
slug: scroll-zkevm-domain-security
source_filename: scroll-zkevm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scroll.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:32:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.scroll.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:39:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.scroll.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:53:50 2026 GMT\n  hsts: null\ndomains:\n- domain: scroll.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scroll-zkevm/refs/heads/main/security/scroll-zkevm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- zkEVM
- Layer 2
- Ethereum
- Rollup
- Zero Knowledge
- JSON-RPC
- Crypto
- Web3
---
