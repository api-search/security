---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: suborbital.dev
  spf: false
hosts:
- cert_expires: Oct 13 16:41:42 2026 GMT
  host: suborbital.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suborbital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suborbital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Suborbital
provider_slug: suborbital
slug: suborbital-domain-security
source_filename: suborbital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suborbital.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 16:41:42 2026 GMT\n  hsts: false\ndomains:\n- domain: suborbital.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suborbital/refs/heads/main/security/suborbital-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Developer Tools
- WebAssembly
- Edge Compute
- Serverless
- Plugins
- Extensibility
---
