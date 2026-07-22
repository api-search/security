---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firnas.aero
  spf: true
hosts:
- cert_expires: Sep 27 06:13:16 2026 GMT
  host: firnas.aero
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firnas Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firnas Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Firnas Aero
provider_slug: firnas-aero
slug: firnas-aero-domain-security
source_filename: firnas-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firnas.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:13:16 2026 GMT\n  hsts: false\ndomains:\n- domain: firnas.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firnas-aero/refs/heads/main/security/firnas-aero-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Drones
- UAV
- Aerial Surveillance
- Industrial Inspection
- Machine Learning
- Robotics
- Saudi Arabia
---
