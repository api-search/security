---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hunters.ai
  spf: true
hosts:
- cert_expires: Sep 21 23:31:03 2026 GMT
  host: www.hunters.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hunters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hunters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hunters
provider_slug: hunters
slug: hunters-domain-security
source_filename: hunters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hunters.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:31:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hunters.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunters/refs/heads/main/security/hunters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- SIEM
- SOC
- Threat Detection
- Security Operations
- Incident Response
- Threat Hunting
---
