---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: credencemed.com
  spf: true
hosts:
- cert_expires: Nov  5 20:25:05 2026 GMT
  host: www.credencemed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credence Medsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credence MedSystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Credence MedSystems
provider_slug: credence-medsystems
slug: credence-medsystems-domain-security
source_filename: credence-medsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credencemed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 20:25:05 2026 GMT\n  hsts: false\ndomains:\n- domain: credencemed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credence-medsystems/refs/heads/main/security/credence-medsystems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Integration
- Middleware
---
