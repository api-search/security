---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dinogame.gg
  spf: true
hosts:
- cert_expires: Dec 23 18:24:50 2026 GMT
  host: dinogame.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dinogame-gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dinogame-gg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dinogame-gg
provider_slug: dinogame-gg
slug: dinogame-gg-domain-security
source_filename: dinogame-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dinogame.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:24:50 2026 GMT\n  hsts: false\ndomains:\n- domain: dinogame.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dinogame-gg/security/dinogame-gg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Games
- Free
- Browser
- No-Tracking
---
