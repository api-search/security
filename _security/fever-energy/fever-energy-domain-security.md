---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fever.energy
  spf: true
hosts:
- cert_expires: Jan 12 22:18:23 2027 GMT
  host: www.fever.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fever Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fever
provider_slug: fever-energy
slug: fever-energy-domain-security
source_filename: fever-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fever.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 22:18:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fever.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fever-energy/security/fever-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Platform
- Distributed-Resources
- API
---
