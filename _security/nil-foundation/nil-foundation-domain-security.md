---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nil.foundation
  spf: true
hosts:
- cert_expires: Oct  1 10:50:45 2026 GMT
  host: nil.foundation
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 19:42:13 2026 GMT
  host: docs.nil.foundation
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.devnet.nil.foundation
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.devnet.'
kind: domain-security
layout: security
method: probed
name: Nil Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for =nil; Foundation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: =nil; Foundation
provider_slug: nil-foundation
slug: nil-foundation-domain-security
source_filename: nil-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nil.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:50:45 2026 GMT\n  hsts: false\n- host: docs.nil.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.devnet.nil.foundation\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.devnet.'\n  hsts: null\ndomains:\n- domain: nil.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nil-foundation/refs/heads/main/security/nil-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Zk Infrastructure
- Blockchain
- Layer 2
- Ethereum
- Zero Knowledge Proofs
- zkSharding
- JSON-RPC
- Smart Contracts
- Developer Tools
---
