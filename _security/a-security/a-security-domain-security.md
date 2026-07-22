---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: a.security
  spf: true
hosts:
- cert_expires: Aug 19 17:48:44 2026 GMT
  host: a.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: A Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: A Security
provider_slug: a-security
slug: a-security-domain-security
source_filename: a-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a.security\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 17:48:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: a.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-security/refs/heads/main/security/a-security-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Offensive Security
- Penetration Testing
- Attack Path Management
- Autonomous Remediation
- AI Security
- Vulnerability Management
---
