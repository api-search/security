---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astral.sh
  spf: true
hosts:
- cert_expires: Oct 12 02:32:31 2026 GMT
  host: astral.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astral, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astral
provider_slug: astral
slug: astral-domain-security
source_filename: astral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astral.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 02:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: astral.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astral/refs/heads/main/security/astral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Python
- Package Manager
- Linter
- Code Formatter
- Type Checker
- CLI
- Open Source
- Rust
---
