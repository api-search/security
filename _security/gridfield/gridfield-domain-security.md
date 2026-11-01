---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gridfield.co
  spf: true
hosts:
- cert_expires: Jan 16 14:54:27 2027 GMT
  host: gridfield.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gridfield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gridfield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gridfield
provider_slug: gridfield
slug: gridfield-domain-security
source_filename: gridfield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gridfield.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 14:54:27 2027 GMT\n  hsts: false\ndomains:\n- domain: gridfield.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gridfield/security/gridfield-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Supercomputing
- Cloud
- Machine Learning
---
