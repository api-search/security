---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pola.rs
  spf: false
hosts:
- cert_expires: Oct 14 19:29:07 2026 GMT
  host: pola.rs
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Polars
provider_slug: polars
slug: polars-domain-security
source_filename: polars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pola.rs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:29:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pola.rs\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polars/refs/heads/main/security/polars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Apis
- DataFrames
- Data Processing
- Query Engine
- Rust
- Python
- Analytics
- Open Source
---
