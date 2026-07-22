---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: valaratomics.com
  spf: true
hosts:
- cert_expires: Oct  1 08:06:01 2026 GMT
  host: www.valaratomics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valar Atomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valar Atomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Valar Atomics
provider_slug: valar-atomics
slug: valar-atomics-domain-security
source_filename: valar-atomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valaratomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: valaratomics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valar-atomics/refs/heads/main/security/valar-atomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate
- Nuclear Energy
- Energy
- Hydrogen
- Synthetic Fuels
- Small Modular Reactors
---
