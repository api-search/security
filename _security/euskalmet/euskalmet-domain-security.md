---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: euskadi.eus
  spf: true
hosts:
- cert_expires: Feb 14 11:15:33 2027 GMT
  host: opendata.euskadi.eus
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Euskalmet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Euskalmet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Euskalmet
provider_slug: euskalmet
slug: euskalmet-domain-security
source_filename: euskalmet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.euskadi.eus\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 11:15:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: euskadi.eus\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euskalmet/refs/heads/main/security/euskalmet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Public APIs
---
