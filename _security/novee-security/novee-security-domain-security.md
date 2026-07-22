---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novee.security
  spf: true
hosts:
- cert_expires: Oct  1 22:14:40 2026 GMT
  host: novee.security
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novee Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novee Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Novee Security
provider_slug: novee-security
slug: novee-security-domain-security
source_filename: novee-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novee.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:14:40 2026 GMT\n  hsts: false\ndomains:\n- domain: novee.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novee-security/refs/heads/main/security/novee-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Penetration Testing
- AI
- Application Security
- DAST
- Red Teaming
- Bug Bounty
- Compliance
- Vulnerability Management
---
