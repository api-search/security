---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swarm.aero
  spf: true
hosts:
- cert_expires: Nov 26 18:37:20 2026 GMT
  host: www.swarm.aero
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swarm Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swarm Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swarm Aero
provider_slug: swarm-aero
slug: swarm-aero-domain-security
source_filename: swarm-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swarm.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 18:37:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swarm.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/swarm-aero/security/swarm-aero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Long‑Range Strike
- Defense
- C2 Autonomy
- Modular Payload
- Mass Production
---
