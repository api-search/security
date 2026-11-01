---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: studeo.app
  spf: true
hosts:
- cert_expires: Dec 20 10:37:54 2026 GMT
  host: studeo.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Studeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Studeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Studeo
provider_slug: studeo
slug: studeo-domain-security
source_filename: studeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: studeo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:37:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: studeo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/studeo/security/studeo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- AI
- Tutoring
- PersonalizedLearning
- SaaS
- Company
---
