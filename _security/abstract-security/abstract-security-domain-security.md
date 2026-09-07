---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abstract.security
  spf: true
hosts:
- cert_expires: Nov 13 12:48:10 2026 GMT
  host: www.abstract.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abstract Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abstract Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abstract Security
provider_slug: abstract-security
slug: abstract-security-domain-security
source_filename: abstract-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abstract.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 12:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abstract.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract-security/refs/heads/main/security/abstract-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Cybersecurity
- SIEM
- Security Data Pipeline
- Threat Detection
- Security Operations
- Log Management
- Data Streaming
- Observability
- Threat Intelligence
- Cloud Security
- AI Security
- Detection Engineering
- Data Routing
- Compliance Retention
---
