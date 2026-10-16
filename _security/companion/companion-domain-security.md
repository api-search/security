---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: companion.ai
  spf: true
hosts:
- cert_expires: Nov 16 11:36:56 2026 GMT
  host: companion.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Companion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Companion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Companion
provider_slug: companion
slug: companion-domain-security
source_filename: companion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: companion.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 11:36:56 2026 GMT\n  hsts: false\ndomains:\n- domain: companion.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companion/refs/heads/main/security/companion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- communication
- interface
- intelligence
- platform
---
