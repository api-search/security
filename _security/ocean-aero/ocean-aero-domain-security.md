---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: oceanaero.com
  spf: true
hosts:
- cert_expires: Nov 21 13:05:58 2026 GMT
  host: www.oceanaero.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocean Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocean Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ocean Aero
provider_slug: ocean-aero
slug: ocean-aero-domain-security
source_filename: ocean-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oceanaero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 13:05:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: oceanaero.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-aero/refs/heads/main/security/ocean-aero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Maritime
- Autonomous Vehicles
- Uncrewed Systems
- Robotics
- Ocean Data
- Defense
- Hardware
---
