---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nippy.host
  spf: true
hosts:
- cert_expires: Jan 23 12:41:37 2027 GMT
  host: nippy.host
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nippy.host Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nippy.host, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nippy.host
provider_slug: nippy-host
slug: nippy-host-domain-security
source_filename: nippy-host-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nippy.host\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:41:37 2027 GMT\n  hsts: false\ndomains:\n- domain: nippy.host\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nippy-host/security/nippy-host-domain-security.yml
summary_line: TLSv1.3
tags:
- Hosting
- File Sharing
- Web Service
- Cloud
- Free Tier
---
