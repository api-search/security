---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eos-aus.com
  spf: true
hosts:
- cert_expires: Dec  6 10:10:07 2026 GMT
  host: eos-aus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Electro Optic Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electro Optic Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Electro Optic Systems
provider_slug: electro-optic-systems
slug: electro-optic-systems-domain-security
source_filename: electro-optic-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eos-aus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 10:10:07 2026 GMT\n  hsts: false\ndomains:\n- domain: eos-aus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electro-optic-systems/refs/heads/main/security/electro-optic-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defence
- Aerospace
- Space
- Counter-Drone
- Laser Weapons
- Remote Weapon Systems
- Australia
---
