---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sillytavern.app
  spf: true
hosts:
- cert_expires: Nov 20 15:16:47 2026 GMT
  host: docs.sillytavern.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sillytavernai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SillyTavern AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SillyTavern AI
provider_slug: sillytavernai
slug: sillytavernai-domain-security
source_filename: sillytavernai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sillytavern.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 15:16:47 2026 GMT\n  hsts: false\ndomains:\n- domain: sillytavern.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/sillytavernai/security/sillytavernai-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Chatbots
- Open Source
- RolePlaying
- Community
---
