---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: justicetext.com
  spf: true
hosts:
- cert_expires: Oct 17 19:05:50 2026 GMT
  host: justicetext.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justicetext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JusticeText, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JusticeText
provider_slug: justicetext
slug: justicetext-domain-security
source_filename: justicetext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justicetext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 19:05:50 2026 GMT\n  hsts: null\ndomains:\n- domain: justicetext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justicetext/refs/heads/main/security/justicetext-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal
- Legal Tech
- Criminal Justice
- Evidence Management
- Transcription
- Artificial Intelligence
- Public Defenders
---
