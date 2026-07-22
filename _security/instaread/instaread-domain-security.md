---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: instaread.co
  spf: false
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: instaread.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instaread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instaread, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Instaread
provider_slug: instaread
slug: instaread-domain-security
source_filename: instaread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instaread.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: instaread.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instaread/refs/heads/main/security/instaread-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Audio
- Text-to-Speech
- Publishing
- Media
- Accessibility
- Book Summaries
- WordPress
---
