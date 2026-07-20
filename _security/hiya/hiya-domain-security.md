---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hiya.com
  spf: true
hosts:
- cert_expires: Oct 15 00:44:10 2026 GMT
  host: hiya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hiya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hiya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hiya
provider_slug: hiya
slug: hiya-domain-security
source_filename: hiya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hiya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiya/refs/heads/main/security/hiya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Voice Security
- Caller ID
- Branded Calling
- Spam Protection
- Scam Protection
- Deepfake Detection
- Voice Authentication
- Telecommunications
- Call Analytics
---
