---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thesparkle.ai
  spf: true
hosts:
- cert_expires: Feb  1 05:34:16 2027 GMT
  host: thesparkle.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thesparkle Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TAAI Labs, Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TAAI Labs, Inc
provider_slug: thesparkle-ai
slug: thesparkle-ai-domain-security
source_filename: thesparkle-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesparkle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 05:34:16 2027 GMT\n  hsts: null\ndomains:\n- domain: thesparkle.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thesparkle-ai/security/thesparkle-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Security
- SDLC
- Platform
---
