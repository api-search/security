---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vention.io
  spf: true
hosts:
- cert_expires: Aug 22 06:14:26 2026 GMT
  host: vention.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vention Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vention, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vention
provider_slug: vention
slug: vention-domain-security
source_filename: vention-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vention.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:14:26 2026 GMT\n  hsts: false\ndomains:\n- domain: vention.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vention/refs/heads/main/security/vention-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Physical Ai
- Manufacturing
- Industrial Automation
- Robotics
- Motion Control
- Python SDK
- Digital Twin
---
