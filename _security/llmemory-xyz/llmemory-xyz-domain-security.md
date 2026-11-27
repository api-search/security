---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: llmemory.xyz
  spf: true
hosts:
- cert_expires: Jan 25 17:12:23 2027 GMT
  host: llmemory.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LLMemory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLMemory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LLMemory
provider_slug: llmemory-xyz
slug: llmemory-xyz-domain-security
source_filename: llmemory-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmemory.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 17:12:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: llmemory.xyz\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/llmemory-xyz/security/llmemory-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat Storage
- Browser Extension
- Privacy
---
