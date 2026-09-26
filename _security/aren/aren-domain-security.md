---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getaren.com
  spf: false
hosts:
- cert_expires: Dec 15 19:27:35 2026 GMT
  host: www.getaren.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aren, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aren
provider_slug: aren
slug: aren-domain-security
source_filename: aren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getaren.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 19:27:35 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: getaren.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aren/refs/heads/main/security/aren-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Recruiting
- Education
- Sports
---
