---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kazkar.ai
  spf: false
hosts:
- cert_expires: Jan 13 19:13:18 2027 GMT
  host: kazkar.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kazkar.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kazkar.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kazkar.ai
provider_slug: kazkar-ai
slug: kazkar-ai-domain-security
source_filename: kazkar-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kazkar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 19:13:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kazkar.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kazkar-ai/security/kazkar-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Discord Bot
- Lore Wiki
- Relationship Graph
---
