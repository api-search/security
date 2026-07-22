---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: transcrypts.com
  spf: true
hosts:
- cert_expires: Sep 16 06:35:50 2026 GMT
  host: www.transcrypts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transcrypts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransCrypts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TransCrypts
provider_slug: transcrypts
slug: transcrypts-domain-security
source_filename: transcrypts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transcrypts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:35:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transcrypts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcrypts/refs/heads/main/security/transcrypts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Identity
- Verification
- Credentials
- Background Checks
- Employment Verification
- Self-Sovereign Data
- HIPAA
---
