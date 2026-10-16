---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: celestiai.co
  spf: true
hosts:
- cert_expires: Dec 29 09:32:30 2026 GMT
  host: celestiai.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celestialai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celestialai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Celestialai
provider_slug: celestialai
slug: celestialai-domain-security
source_filename: celestialai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celestiai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 09:32:30 2026 GMT\n  hsts: false\ndomains:\n- domain: celestiai.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celestialai/refs/heads/main/security/celestialai-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Content
- Short-form Video
- Content Calendar
- Voice Cloning
---
