---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cenos-platform.com
  spf: true
hosts:
- cert_expires: Sep  7 02:14:38 2026 GMT
  host: cenos-platform.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cenos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cenos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cenos
provider_slug: cenos
slug: cenos-domain-security
source_filename: cenos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cenos-platform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:14:38 2026 GMT\n  hsts: false\ndomains:\n- domain: cenos-platform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cenos/refs/heads/main/security/cenos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Simulation
- Engineering
- Electromagnetics
- Induction Heating
- Radio Frequency
- Wireless Charging
- CAE
- FEM
---
