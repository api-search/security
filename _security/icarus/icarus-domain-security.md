---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: icarus.one
  spf: true
hosts:
- cert_expires: Sep 26 05:03:15 2026 GMT
  host: www.icarus.one
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icarus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Icarus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Icarus
provider_slug: icarus
slug: icarus-domain-security
source_filename: icarus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icarus.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: icarus.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icarus/refs/heads/main/security/icarus-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Aerospace
- Defense
- Surveillance
- Connectivity
- Stratospheric
- Autonomous Aircraft
- Solar Power
---
