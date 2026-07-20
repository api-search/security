---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lingco.io
  spf: true
hosts:
- cert_expires: Oct  4 11:26:08 2026 GMT
  host: lingco.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 16:19:49 2026 GMT
  host: help.lingco.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 16:19:49 2026 GMT
  host: class.lingco.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lingco Language Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lingco Language Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lingco Language Labs
provider_slug: lingco-language-labs
slug: lingco-language-labs-domain-security
source_filename: lingco-language-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lingco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.lingco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:19:49 2026 GMT\n  hsts: false\n- host: class.lingco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:19:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lingco.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingco-language-labs/refs/heads/main/security/lingco-language-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Language Learning
- Learning Management
- LTI
- OneRoster
- Rostering
- Single Sign On
- Interoperability
---
