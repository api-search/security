---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: justmeme.wtf
  spf: true
hosts:
- cert_expires: Oct  4 05:46:37 2026 GMT
  host: justmeme.wtf
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justmeme Wtf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for justmeme.wtf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: justmeme.wtf
provider_slug: justmeme-wtf
slug: justmeme-wtf-domain-security
source_filename: justmeme-wtf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justmeme.wtf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: justmeme.wtf\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justmeme-wtf/refs/heads/main/security/justmeme-wtf-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Entertainment
- Public APIs
---
