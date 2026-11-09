---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: art-deco-belgique.be
  spf: true
hosts:
- cert_expires: Dec 11 02:23:47 2026 GMT
  host: art-deco-belgique.be
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Art Deco Belgique Be Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Art Déco Belgique, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Art Déco Belgique
provider_slug: art-deco-belgique-be
slug: art-deco-belgique-be-domain-security
source_filename: art-deco-belgique-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: art-deco-belgique.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: art-deco-belgique.be\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/art-deco-belgique-be/security/art-deco-belgique-be-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Art Deco
- Heritage
- Belgium
- Architecture
- Open Data
---
