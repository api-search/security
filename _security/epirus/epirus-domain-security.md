---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epirusinc.com
  spf: true
hosts:
- cert_expires: Aug 16 07:43:34 2026 GMT
  host: www.epirusinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epirus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epirus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Epirus
provider_slug: epirus
slug: epirus-domain-security
source_filename: epirus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epirusinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:43:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epirusinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epirus/refs/heads/main/security/epirus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Defense
- Defense Technology
- Directed Energy
- High-Power Microwave
- Counter-UAS
- Counter-Drone
- Counter-Electronics
- Electronic Warfare
- Non-Kinetic Effects
- Air Defense
- Air Domain Awareness
- National Security
- Government
- Military
- Leonidas
- IFPC-HPM
- Hardware
---
