---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apimetro.dev
  spf: false
hosts:
- cert_expires: Sep 11 22:32:01 2026 GMT
  host: apimetro.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apimetro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apimetro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Apimetro
provider_slug: apimetro
slug: apimetro-domain-security
source_filename: apimetro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apimetro.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 22:32:01 2026 GMT\n  hsts: null\ndomains:\n- domain: apimetro.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimetro/refs/heads/main/security/apimetro-domain-security.yml
summary_line: TLSv1.3
tags:
- Transportation
- Public APIs
---
