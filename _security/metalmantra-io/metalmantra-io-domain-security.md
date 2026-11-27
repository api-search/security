---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metalmantra.io
  spf: true
hosts:
- cert_expires: Jan  5 00:25:27 2027 GMT
  host: metalmantra.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: metalmantra-io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for metalmantra-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: metalmantra-io
provider_slug: metalmantra-io
slug: metalmantra-io-domain-security
source_filename: metalmantra-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metalmantra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:25:27 2027 GMT\n  hsts: null\ndomains:\n- domain: metalmantra.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/metalmantra-io/security/metalmantra-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
