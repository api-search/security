---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gem.security
  spf: true
hosts:
- cert_expires: Sep 23 07:56:15 2026 GMT
  host: www.gem.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gem
provider_slug: gem
slug: gem-domain-security
source_filename: gem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gem.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:56:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gem.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gem/refs/heads/main/security/gem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud Security
- Cloud Detection and Response
- CDR
- Threat Detection
- Acquired
---
