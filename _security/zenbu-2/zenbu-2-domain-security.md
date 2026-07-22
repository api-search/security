---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: tryzenbu.dev
  spf: false
hosts:
- cert_expires: Sep  2 21:06:37 2026 GMT
  host: tryzenbu.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenbu 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenbu 2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zenbu 2
provider_slug: zenbu-2
slug: zenbu-2-domain-security
source_filename: zenbu-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryzenbu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:06:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tryzenbu.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenbu-2/refs/heads/main/security/zenbu-2-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Developer Tools
- AI Coding Agents
- Frameworks
- SDK
- Open Source
- Desktop Application
- Y Combinator
---
