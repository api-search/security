---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: superfeedr.com
  spf: true
hosts:
- cert_expires: Nov 30 05:07:11 2026 GMT
  host: superfeedr.com
  hsts: true
  hsts_max_age: 631152000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Superfeedr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superfeedr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Superfeedr
provider_slug: superfeedr
slug: superfeedr-domain-security
source_filename: superfeedr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superfeedr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 05:07:11 2026 GMT\n  hsts: true\n  hsts_max_age: 631152000\ndomains:\n- domain: superfeedr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superfeedr/refs/heads/main/security/superfeedr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Real-time
- Feed
- API
- PubSubHubbub
---
