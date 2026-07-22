---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voidzero.dev
  spf: true
hosts:
- cert_expires: Aug 31 02:41:56 2026 GMT
  host: voidzero.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voidzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VoidZero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VoidZero
provider_slug: voidzero
slug: voidzero-domain-security
source_filename: voidzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voidzero.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:41:56 2026 GMT\n  hsts: false\ndomains:\n- domain: voidzero.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voidzero/refs/heads/main/security/voidzero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- JavaScript
- Build Tools
- Toolchain
- Open Source
- Testing
- Bundler
---
