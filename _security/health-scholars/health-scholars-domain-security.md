---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upskillai.com
  spf: true
hosts:
- cert_expires: Nov 11 14:02:14 2026 GMT
  host: upskillai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Health Scholars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Health Scholars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Health Scholars
provider_slug: health-scholars
slug: health-scholars-domain-security
source_filename: health-scholars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upskillai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:02:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upskillai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-scholars/refs/heads/main/security/health-scholars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Training
- Simulation
- Virtual Reality
- Extended Reality
- Healthcare
- Education
- Defense
- Emergency Medical Services
- Artificial Intelligence
---
