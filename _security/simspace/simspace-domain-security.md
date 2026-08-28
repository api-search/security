---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simspace.com
  spf: true
hosts:
- cert_expires: Nov  2 19:15:36 2026 GMT
  host: simspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 19:15:36 2026 GMT
  host: portal.simspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimSpace, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SimSpace
provider_slug: simspace
slug: simspace-domain-security
source_filename: simspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:15:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.simspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:15:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simspace/refs/heads/main/security/simspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Cyber Range
- Security Training
- Simulation
- AI Agents
- Security Operations
- Critical Infrastructure
- Government
- Compliance
---
