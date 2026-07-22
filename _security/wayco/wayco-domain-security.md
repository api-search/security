---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wayco.ai
  spf: false
hosts:
- cert_expires: Oct 11 15:31:01 2026 GMT
  host: wayco.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wayco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wayco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Wayco
provider_slug: wayco
slug: wayco-domain-security
source_filename: wayco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wayco.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 15:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wayco.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayco/refs/heads/main/security/wayco-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Legal Tech
- Artificial Intelligence
- Healthcare
- Voice AI
- Case Management
- Personal Injury
- Insurance
---
