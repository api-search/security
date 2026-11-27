---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: halite.cc
  spf: true
hosts:
- cert_expires: Jan  3 16:34:24 2027 GMT
  host: halite.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: halite-cc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for halite-cc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: halite-cc
provider_slug: halite-cc
slug: halite-cc-domain-security
source_filename: halite-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: halite.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 16:34:24 2027 GMT\n  hsts: false\ndomains:\n- domain: halite.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/halite-cc/security/halite-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Recipe Manager
- Meal Planning
- Grocery List
- Cooking App
- Recipe Import
---
