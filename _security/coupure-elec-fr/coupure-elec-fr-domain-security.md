---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coupure-elec.fr
  spf: false
hosts:
- cert_expires: Jan  8 06:47:45 2027 GMT
  host: coupure-elec.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coupure-Elec.fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coupure-Elec.fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Coupure-Elec.fr
provider_slug: coupure-elec-fr
slug: coupure-elec-fr-domain-security
source_filename: coupure-elec-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coupure-elec.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 06:47:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coupure-elec.fr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coupure-elec-fr/security/coupure-elec-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electricity
- Power Outages
- Energy
- France
- MCP
- Crowdsourcing
- Open Data
---
