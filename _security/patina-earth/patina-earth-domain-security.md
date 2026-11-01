---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: patina.earth
  spf: true
hosts:
- cert_expires: Jan 28 23:07:34 2027 GMT
  host: patina.earth
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Patina Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Patina
provider_slug: patina-earth
slug: patina-earth-domain-security
source_filename: patina-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patina.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:07:34 2027 GMT\n  hsts: false\ndomains:\n- domain: patina.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/patina-earth/security/patina-earth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fragrance
- Flavor
- Perfumery
- Molecular Design
- Machine Learning
- Olfactory Technology
---
