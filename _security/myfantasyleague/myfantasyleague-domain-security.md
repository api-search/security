---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myfantasyleague.com
  spf: true
hosts:
- cert_expires: Nov 22 17:54:50 2026 GMT
  host: myfantasyleague.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Myfantasyleague Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyFantasyLeague API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyFantasyLeague API
provider_slug: myfantasyleague
slug: myfantasyleague-domain-security
source_filename: myfantasyleague-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myfantasyleague.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 17:54:50 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: myfantasyleague.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myfantasyleague/security/myfantasyleague-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fantasy Sports
- Football
- League Management
- Custom Scoring
- Community
---
