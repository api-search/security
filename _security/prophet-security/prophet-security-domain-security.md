---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prophetsecurity.ai
  spf: true
hosts:
- cert_expires: Sep 12 12:03:35 2026 GMT
  host: www.prophetsecurity.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prophet Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prophet Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prophet Security
provider_slug: prophet-security
slug: prophet-security-domain-security
source_filename: prophet-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prophetsecurity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:03:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prophetsecurity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prophet-security/refs/heads/main/security/prophet-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Security
- Cybersecurity
- SOC
- Security Operations
- Threat Detection
- Agentic AI
---
