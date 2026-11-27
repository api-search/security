---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ownyourai.app
  spf: true
hosts:
- cert_expires: Feb 15 19:26:46 2027 GMT
  host: ownyourai.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Own Your AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Own Your AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Own Your AI
provider_slug: ownyourai-app
slug: ownyourai-app-domain-security
source_filename: ownyourai-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ownyourai.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 19:26:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ownyourai.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ownyourai-app/security/ownyourai-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Tools
- Voice-to-Text
- Private AI
- Mac Software
- Founding Membership
- Open‑source Packaging
---
