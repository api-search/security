---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lean-lang.org
  spf: false
hosts:
- cert_expires: Sep 22 07:03:47 2026 GMT
  host: lean-lang.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lean, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Lean
provider_slug: lean
slug: lean-domain-security
source_filename: lean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lean-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lean-lang.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean/refs/heads/main/security/lean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Dependent Types
- Formal Verification
- Programming Language
- Theorem Prover
---
