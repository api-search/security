---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: circuitlab.com
  spf: true
hosts:
- cert_expires: Sep 18 14:17:55 2026 GMT
  host: www.circuitlab.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Circuitlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CircuitLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CircuitLab
provider_slug: circuitlab
slug: circuitlab-domain-security
source_filename: circuitlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.circuitlab.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 14:17:55 2026 GMT\n  hsts: false\ndomains:\n- domain: circuitlab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuitlab/refs/heads/main/security/circuitlab-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Electronics
- Circuit Simulation
- Schematic Capture
- EDA
- Simulation
- Engineering
- Education
---
