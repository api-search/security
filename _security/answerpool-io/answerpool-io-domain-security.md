---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: answerpool.io
  spf: true
hosts:
- cert_expires: Jan 27 03:27:30 2027 GMT
  host: answerpool.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: answerpool-io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for answerpool-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: answerpool-io
provider_slug: answerpool-io
slug: answerpool-io-domain-security
source_filename: answerpool-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: answerpool.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 03:27:30 2027 GMT\n  hsts: null\ndomains:\n- domain: answerpool.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/answerpool-io/security/answerpool-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
