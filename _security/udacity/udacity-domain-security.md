---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: udacity.com
  spf: true
hosts:
- cert_expires: Aug 23 10:43:23 2026 GMT
  host: www.udacity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Udacity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Udacity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Udacity
provider_slug: udacity
slug: udacity-domain-security
source_filename: udacity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.udacity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:43:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: udacity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/udacity/refs/heads/main/security/udacity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Online Learning
- Upskilling
- Nanodegrees
- Tech Education
- Workforce Development
- Generative AI Training
- Agentic AI
- Data Science
- Cloud Computing
- Cybersecurity
- Autonomous Systems
- Self-Driving Cars
- Accenture
- LearnVantage
---
