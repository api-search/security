---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fiveable.me
  spf: true
hosts:
- cert_expires: Oct  9 12:32:13 2026 GMT
  host: fiveable.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fiveable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiveable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fiveable
provider_slug: fiveable
slug: fiveable-domain-security
source_filename: fiveable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiveable.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:32:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fiveable.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiveable/refs/heads/main/security/fiveable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- EdTech
- AP Exam Prep
- Study Tools
- Practice Questions
- AI Scoring
- Students
---
