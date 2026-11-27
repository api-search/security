---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drapecut.com
  spf: true
hosts:
- cert_expires: Jan 28 10:46:47 2027 GMT
  host: drapecut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DrapeCut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DrapeCut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DrapeCut
provider_slug: drapecut-com
slug: drapecut-com-domain-security
source_filename: drapecut-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drapecut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:46:47 2027 GMT\n  hsts: null\ndomains:\n- domain: drapecut.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/drapecut-com/security/drapecut-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Engineering
- Simulation
- Composite
- Fabric
- DXF
---
