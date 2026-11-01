---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: compgen.de
  spf: true
hosts:
- cert_expires: Jan 15 16:05:21 2027 GMT
  host: compgen.de
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compgen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompGen DES / domus.genealogy.net historical building map, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CompGen DES / domus.genealogy.net historical building map
provider_slug: compgen
slug: compgen-domain-security
source_filename: compgen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compgen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 16:05:21 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: compgen.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/compgen/security/compgen-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Genealogy
- History
- Data
- Non-profit
- Germany
---
