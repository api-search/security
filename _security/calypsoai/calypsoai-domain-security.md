---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: calypsoai.org
  spf: false
hosts:
- cert_expires: Nov  6 00:16:20 2026 GMT
  host: calypsoai.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calypsoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CalypsoAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CalypsoAI
provider_slug: calypsoai
slug: calypsoai-domain-security
source_filename: calypsoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calypsoai.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 00:16:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: calypsoai.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calypsoai/refs/heads/main/security/calypsoai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Call Answering
- Home Services
- HVAC
- Plumbing
- AI Dispatch
---
