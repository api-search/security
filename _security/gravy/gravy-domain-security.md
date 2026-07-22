---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gravy.finance
  spf: false
hosts:
- cert_expires: Oct 12 05:16:22 2026 GMT
  host: gravy.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gravy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gravy
provider_slug: gravy
slug: gravy-domain-security
source_filename: gravy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gravy.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gravy.finance\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravy/refs/heads/main/security/gravy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Personal Finance
- Fintech
- AI
- Consumer
- Local-First
- Mac
- Financial Management
---
