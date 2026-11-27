---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: groovalizer.space
  spf: false
hosts:
- cert_expires: Dec 28 06:07:29 2026 GMT
  host: groovalizer.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Groovalizer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groovalizer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Groovalizer
provider_slug: groovalizer-space
slug: groovalizer-space-domain-security
source_filename: groovalizer-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groovalizer.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 06:07:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: groovalizer.space\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/groovalizer-space/security/groovalizer-space-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Audio
- Video
- Music
- Visualizer
- Social Media
---
