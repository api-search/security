---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cfl.ca
  spf: true
hosts:
- host: api.cfl.ca
  https: false
kind: domain-security
layout: security
method: probed
name: Canadian Football League Cfl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canadian Football League (CFL), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Canadian Football League (CFL)
provider_slug: canadian-football-league-cfl
slug: canadian-football-league-cfl-domain-security
source_filename: canadian-football-league-cfl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.cfl.ca\n  https: false\ndomains:\n- domain: cfl.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-football-league-cfl/refs/heads/main/security/canadian-football-league-cfl-domain-security.yml
summary_line: DMARC
tags:
- Sports And Fitness
- Public APIs
---
