---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: multitracks.com
  spf: true
hosts:
- cert_expires: Feb 13 21:16:22 2027 GMT
  host: www.multitracks.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RehearsalMix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RehearsalMix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RehearsalMix
provider_slug: rehearsalmix
slug: rehearsalmix-domain-security
source_filename: rehearsalmix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.multitracks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 21:16:22 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: multitracks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rehearsalmix/security/rehearsalmix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Collaboration
- Audio
- Rehearsal
- Platform
---
