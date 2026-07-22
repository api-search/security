---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sv.academy
  spf: true
hosts:
- cert_expires: Oct  9 04:58:50 2026 GMT
  host: www.sv.academy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sv Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SV Academy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SV Academy
provider_slug: sv-academy
slug: sv-academy-domain-security
source_filename: sv-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sv.academy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:58:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sv.academy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sv-academy/refs/heads/main/security/sv-academy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Training
- Talent Placement
- Sales Development
- Workforce Development
- Career Services
---
