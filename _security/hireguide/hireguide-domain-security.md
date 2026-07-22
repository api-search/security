---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hireguide.com
  spf: false
hosts:
- cert_expires: Sep 12 03:39:11 2026 GMT
  host: hireguide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hireguide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hireguide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hireguide
provider_slug: hireguide
slug: hireguide-domain-security
source_filename: hireguide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hireguide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:39:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hireguide.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hireguide/refs/heads/main/security/hireguide-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Hiring
- Recruiting
- Interviewing
- Talent Acquisition
- HR Tech
- AI
- Structured Interviews
---
