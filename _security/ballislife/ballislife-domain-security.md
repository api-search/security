---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ballislife.com
  spf: true
hosts:
- cert_expires: Nov 10 14:54:05 2026 GMT
  host: ballislife.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ballislife Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ballislife, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ballislife
provider_slug: ballislife
slug: ballislife-domain-security
source_filename: ballislife-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ballislife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 14:54:05 2026 GMT\n  hsts: false\ndomains:\n- domain: ballislife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ballislife/refs/heads/main/security/ballislife-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sports
- Media
- Basketball
- Community
---
