---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: quizlet.com
  spf: true
hosts:
- cert_expires: Sep 23 16:17:28 2026 GMT
  host: quizlet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quizlet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quizlet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Quizlet
provider_slug: quizlet
slug: quizlet-domain-security
source_filename: quizlet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quizlet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:17:28 2026 GMT\n  hsts: false\ndomains:\n- domain: quizlet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quizlet/refs/heads/main/security/quizlet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- EdTech
- Learning
- Study Tools
- Flashcards
- Practice Tests
- Spaced Repetition
- Adaptive Learning
- AI Tutor
- Magic Notes
- Classroom
- Teachers
- Students
---
