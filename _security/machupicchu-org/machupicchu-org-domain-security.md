---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: machupicchu.org
  spf: true
hosts:
- cert_expires: Jan  4 05:56:52 2027 GMT
  host: machupicchu.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Machu Picchu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machu Picchu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Machu Picchu
provider_slug: machupicchu-org
slug: machupicchu-org-domain-security
source_filename: machupicchu-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machupicchu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 05:56:52 2027 GMT\n  hsts: false\ndomains:\n- domain: machupicchu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/machupicchu-org/security/machupicchu-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Heritage
- Guides
- Tourism
- Peru
---
