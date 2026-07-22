---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: emonomy.xyz
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: emonomy.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emonomy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emonomy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Emonomy
provider_slug: emonomy
slug: emonomy-domain-security
source_filename: emonomy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emonomy.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: emonomy.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emonomy/refs/heads/main/security/emonomy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
