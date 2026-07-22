---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: luminatech.co
  spf: true
hosts:
- cert_expires: Oct 18 12:21:58 2026 GMT
  host: luminatech.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lumina
provider_slug: lumina
slug: lumina-domain-security
source_filename: lumina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luminatech.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:21:58 2026 GMT\n  hsts: false\ndomains:\n- domain: luminatech.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumina/refs/heads/main/security/lumina-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Construction
- Autonomous Vehicles
- Robotics
- Electric Vehicles
- Heavy Equipment
- Artificial Intelligence
- Hardware
---
