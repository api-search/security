---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: antimatter.systems
  spf: true
hosts:
- cert_expires: Oct 15 01:37:19 2026 GMT
  host: antimatter.systems
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antimatter Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antimatter Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Antimatter Systems
provider_slug: antimatter-systems
slug: antimatter-systems-domain-security
source_filename: antimatter-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antimatter.systems\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:37:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: antimatter.systems\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antimatter-systems/refs/heads/main/security/antimatter-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Learning
- Classroom
- Memes
- Games
- Community
- Consumer
---
