---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: publicsuffix.org
  spf: false
hosts:
- cert_expires: Dec 30 17:47:50 2026 GMT
  host: publicsuffix.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rutorrent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ruTorrent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ruTorrent
provider_slug: rutorrent
slug: rutorrent-domain-security
source_filename: rutorrent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: publicsuffix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 17:47:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: publicsuffix.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rutorrent/security/rutorrent-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- BitTorrent
- OpenSource
- WebUI
- GPLv3
---
