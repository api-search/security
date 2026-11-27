---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reelsongfinder.com
  spf: true
hosts:
- cert_expires: Feb 11 04:17:17 2027 GMT
  host: reelsongfinder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReelSongFinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReelSongFinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ReelSongFinder
provider_slug: reelsongfinder-com
slug: reelsongfinder-com-domain-security
source_filename: reelsongfinder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reelsongfinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 04:17:17 2027 GMT\n  hsts: false\ndomains:\n- domain: reelsongfinder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reelsongfinder-com/security/reelsongfinder-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Song Identification
- Music Metadata
---
