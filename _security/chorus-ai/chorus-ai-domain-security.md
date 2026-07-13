---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chorus.ai
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.chorus.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.chorus.ai
  https: false
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: chorus.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chorus Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chorus.ai, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chorus.ai
provider_slug: chorus-ai
slug: chorus-ai-domain-security
source_filename: chorus-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chorus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: docs.chorus.ai\n  https: false\n- host: chorus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: chorus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/security/chorus-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sales
- Revenue Intelligence
- Conversation
- Analytics
- ZoomInfo
---
