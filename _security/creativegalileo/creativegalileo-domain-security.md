---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: creativegalileo.com
  spf: true
hosts:
- cert_expires: Nov  6 12:49:05 2026 GMT
  host: www.creativegalileo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Creativegalileo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creativegalileo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Creativegalileo
provider_slug: creativegalileo
slug: creativegalileo-domain-security
source_filename: creativegalileo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creativegalileo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 12:49:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: creativegalileo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creativegalileo/refs/heads/main/security/creativegalileo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- EdTech
- EarlyLearning
- India
- Startups
---
