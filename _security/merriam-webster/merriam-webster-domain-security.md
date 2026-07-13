---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dictionaryapi.com
  spf: false
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: dictionaryapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merriam Webster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merriam-Webster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Merriam-Webster
provider_slug: merriam-webster
slug: merriam-webster-domain-security
source_filename: merriam-webster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dictionaryapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dictionaryapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merriam-webster/refs/heads/main/security/merriam-webster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dictionaries
- Public APIs
---
