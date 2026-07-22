---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: simudyne.com
  spf: true
hosts:
- cert_expires: Jan 25 13:04:36 2027 GMT
  host: simudyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simudyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simudyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Simudyne
provider_slug: simudyne
slug: simudyne-domain-security
source_filename: simudyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simudyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 13:04:36 2027 GMT\n  hsts: false\ndomains:\n- domain: simudyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simudyne/refs/heads/main/security/simudyne-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Simulation
- Agent-Based Modeling
- Synthetic Data
- Market Data
- Financial Services
- Machine Learning
- Developer SDK
---
