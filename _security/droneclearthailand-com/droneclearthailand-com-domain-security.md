---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: droneclearthailand.com
  spf: true
hosts:
- cert_expires: Dec 30 06:56:48 2026 GMT
  host: droneclearthailand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DroneClear Thailand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DroneClear Thailand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DroneClear Thailand
provider_slug: droneclearthailand-com
slug: droneclearthailand-com-domain-security
source_filename: droneclearthailand-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: droneclearthailand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 06:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: droneclearthailand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/droneclearthailand-com/security/droneclearthailand-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drone
- Registration
- Thailand
- Compliance
- Services
---
