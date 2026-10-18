---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: creekstone.energy
  spf: true
hosts:
- cert_expires: Jan  5 11:48:22 2027 GMT
  host: www.creekstone.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Creekstoneenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creekstoneenergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Creekstoneenergy
provider_slug: creekstoneenergy
slug: creekstoneenergy-domain-security
source_filename: creekstoneenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creekstone.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 11:48:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: creekstone.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creekstoneenergy/refs/heads/main/security/creekstoneenergy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Artificial Intelligence
- Infrastructure
- Power
---
