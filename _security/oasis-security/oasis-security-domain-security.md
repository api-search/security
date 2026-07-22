---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oasis.security
  spf: true
hosts:
- cert_expires: Sep 30 21:11:26 2026 GMT
  host: oasis.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oasis Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oasis Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oasis Security
provider_slug: oasis-security
slug: oasis-security-domain-security
source_filename: oasis-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oasis.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:11:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oasis.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oasis-security/refs/heads/main/security/oasis-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Non-Human Identity
- Identity Management
- AI Agents
- Cloud Security
- Cybersecurity
---
