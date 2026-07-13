---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crowdstrike.com
  spf: true
hosts:
- cert_expires: Oct  6 07:46:20 2026 GMT
  host: www.crowdstrike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adaptive Shield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptive Shield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Adaptive Shield
provider_slug: adaptive-shield
slug: adaptive-shield-domain-security
source_filename: adaptive-shield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowdstrike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:46:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crowdstrike.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-shield/refs/heads/main/security/adaptive-shield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SaaS Security
- SSPM
- Security Posture Management
- Cybersecurity
- Cloud Security
- Identity Management
- Compliance
---
