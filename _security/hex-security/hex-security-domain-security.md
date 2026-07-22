---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hex.co
  spf: true
hosts:
- cert_expires: Oct 10 14:47:03 2026 GMT
  host: hex.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hex Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hex Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hex Security
provider_slug: hex-security
slug: hex-security-domain-security
source_filename: hex-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hex.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:47:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hex.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex-security/refs/heads/main/security/hex-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Penetration Testing
- Application Security
- API Security
- Vulnerability Management
- Artificial Intelligence
- AI Agents
- DevSecOps
- Y Combinator
---
