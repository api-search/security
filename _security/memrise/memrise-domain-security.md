---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: memrise.com
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.memrise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memrise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memrise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: memrise
provider_slug: memrise
slug: memrise-domain-security
source_filename: memrise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.memrise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: memrise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memrise/refs/heads/main/security/memrise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Language Learning
- Education
- EdTech
- Mobile App
- Consumer
- AI
---
