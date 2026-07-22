---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atomlearning.com
  spf: true
hosts:
- cert_expires: Sep 15 19:52:35 2026 GMT
  host: www.atomlearning.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atom Learning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atom Learning, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atom Learning
provider_slug: atom-learning
slug: atom-learning-domain-security
source_filename: atom-learning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atomlearning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:52:35 2026 GMT\n  hsts: false\ndomains:\n- domain: atomlearning.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom-learning/refs/heads/main/security/atom-learning-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edtech
- Education
- Exam Preparation
- 11 Plus
- Adaptive Learning
- Assessment
- K-12
- United Kingdom
---
