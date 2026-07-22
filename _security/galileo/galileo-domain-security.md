---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: galileo.io
  spf: true
hosts:
- cert_expires: Aug 20 17:41:25 2026 GMT
  host: galileo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galileo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galileo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Galileo
provider_slug: galileo
slug: galileo-domain-security
source_filename: galileo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galileo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:41:25 2026 GMT\n  hsts: false\ndomains:\n- domain: galileo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo/refs/heads/main/security/galileo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Digital Health
- Primary Care
- Multi-Specialty Care
- Value-Based Care
- Virtual Care
- Health Plans
- Employer Health
---
