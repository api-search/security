---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elyza.ai
  spf: true
hosts:
- cert_expires: Jan 11 12:18:38 2027 GMT
  host: elyza.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elyza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELYZA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ELYZA
provider_slug: elyza
slug: elyza-domain-security
source_filename: elyza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elyza.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 12:18:38 2027 GMT\n  hsts: false\ndomains:\n- domain: elyza.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elyza/refs/heads/main/security/elyza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Natural Language Processing
- Enterprise
- Platform
---
