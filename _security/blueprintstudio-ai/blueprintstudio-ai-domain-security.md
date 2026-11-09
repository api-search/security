---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blueprintstudio.ai
  spf: true
hosts:
- cert_expires: Nov 29 11:12:35 2026 GMT
  host: blueprintstudio.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blueprintstudio Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blueprint Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blueprint Studio
provider_slug: blueprintstudio-ai
slug: blueprintstudio-ai-domain-security
source_filename: blueprintstudio-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueprintstudio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 11:12:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blueprintstudio.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blueprintstudio-ai/security/blueprintstudio-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Development
- Branding
- Launch Videos
- Subscription
- UI/UX
- Web Development
- Mobile App
---
