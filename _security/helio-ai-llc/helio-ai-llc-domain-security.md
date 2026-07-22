---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helio-ai.com
  spf: true
hosts:
- cert_expires: Oct 16 23:32:04 2026 GMT
  host: helio-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helio Ai Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helio AI LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Helio AI LLC
provider_slug: helio-ai-llc
slug: helio-ai-llc-domain-security
source_filename: helio-ai-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helio-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:32:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helio-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helio-ai-llc/refs/heads/main/security/helio-ai-llc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Applicant Tracking System
- ATS
- Human Resources
- HR Tech
- Artificial Intelligence
- Talent Acquisition
- SaaS
---
