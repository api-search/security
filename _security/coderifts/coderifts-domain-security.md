---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coderifts.com
  spf: true
hosts:
- cert_expires: Jan  7 11:19:55 2027 GMT
  host: coderifts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coderifts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeRifts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CodeRifts
provider_slug: coderifts
slug: coderifts-domain-security
source_filename: coderifts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coderifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 11:19:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coderifts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coderifts/refs/heads/main/security/coderifts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Verification
- Compliance
- Platform
---
