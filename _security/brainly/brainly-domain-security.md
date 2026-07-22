---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brainly.com
  spf: true
hosts:
- cert_expires: Oct  5 15:29:18 2026 GMT
  host: brainly.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brainly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brainly
provider_slug: brainly
slug: brainly-domain-security
source_filename: brainly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:29:18 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: brainly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainly/refs/heads/main/security/brainly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Education
- EdTech
- Learning
- Homework Help
- AI Tutor
- Community
---
