---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orval.dev
  spf: false
hosts:
- cert_expires: Aug 22 15:29:18 2026 GMT
  host: orval.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orval, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orval
provider_slug: orval
slug: orval-domain-security
source_filename: orval-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orval.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:29:18 2026 GMT\n  hsts: false\ndomains:\n- domain: orval.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orval/refs/heads/main/security/orval-domain-security.yml
summary_line: TLSv1.3
tags:
- Code Generation
- OpenAPI
- SDKs
- TypeScript
---
