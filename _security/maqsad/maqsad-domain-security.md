---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: maqsad.io
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: maqsad.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Maqsad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maqsad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maqsad
provider_slug: maqsad
slug: maqsad-domain-security
source_filename: maqsad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maqsad.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: maqsad.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maqsad/refs/heads/main/security/maqsad-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Test Preparation
- E-Learning
- Pakistan
- Mobile App
- Consumer
---
