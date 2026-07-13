---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: valencesecurity.com
  spf: true
hosts:
- cert_expires: Aug 18 02:24:36 2026 GMT
  host: www.valencesecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valence Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valence Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Valence Security
provider_slug: valence-security
slug: valence-security-domain-security
source_filename: valence-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valencesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:24:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: valencesecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valence-security/refs/heads/main/security/valence-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS Security
- SSPM
- AI Security
- Identity Security
- ITDR
- Posture Management
- Risk Remediation
---
