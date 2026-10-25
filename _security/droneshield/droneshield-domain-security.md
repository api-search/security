---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: droneshield.com
  spf: true
hosts:
- cert_expires: Nov 24 18:20:38 2026 GMT
  host: droneshield.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Droneshield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DroneShield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DroneShield
provider_slug: droneshield
slug: droneshield-domain-security
source_filename: droneshield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: droneshield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 18:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: droneshield.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/droneshield/refs/heads/main/security/droneshield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Counter-Drone
- Defense
- Drones
- Artificial Intelligence
- Security
- ASX Listed
---
