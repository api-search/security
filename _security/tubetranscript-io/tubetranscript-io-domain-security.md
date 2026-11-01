---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tubetranscript.io
  spf: true
hosts:
- cert_expires: Dec 23 09:48:11 2026 GMT
  host: tubetranscript.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tubetranscript Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tubetranscript-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: tubetranscript-io
provider_slug: tubetranscript-io
slug: tubetranscript-io-domain-security
source_filename: tubetranscript-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tubetranscript.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 09:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tubetranscript.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tubetranscript-io/security/tubetranscript-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- YouTube
- Transcript
- FreeTool
- API
---
