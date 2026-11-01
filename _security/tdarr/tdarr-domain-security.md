---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tdarr.io
  spf: true
hosts:
- cert_expires: Jan  3 12:06:10 2027 GMT
  host: tdarr.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tdarr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tdarr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tdarr
provider_slug: tdarr
slug: tdarr-domain-security
source_filename: tdarr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tdarr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:06:10 2027 GMT\n  hsts: false\ndomains:\n- domain: tdarr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tdarr/security/tdarr-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Video
- Transcoding
- Automation
- OpenSource
---
