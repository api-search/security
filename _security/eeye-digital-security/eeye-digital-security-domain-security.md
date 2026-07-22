---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eye.security
  spf: true
hosts:
- cert_expires: Oct 11 17:38:24 2026 GMT
  host: www.eye.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eeye Digital Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eye Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Eye Security
provider_slug: eeye-digital-security
slug: eeye-digital-security-domain-security
source_filename: eeye-digital-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eye.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:38:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eye.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eeye-digital-security/refs/heads/main/security/eeye-digital-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- Managed XDR
- Incident Response
- Cyber Insurance
- Security Awareness
- Endpoint Security
- Europe
---
