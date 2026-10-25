---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: libryo.com
  spf: true
hosts:
- cert_expires: Dec  6 14:05:49 2026 GMT
  host: libryo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.libryo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Libryo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Libryo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Libryo
provider_slug: libryo
slug: libryo-domain-security
source_filename: libryo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: libryo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 14:05:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.libryo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: libryo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libryo/refs/heads/main/security/libryo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Regulatory Compliance
- Legal Tech
- Environmental Health and Safety
- Governance Risk and Compliance
- Legal Registers
- Regulatory Change Management
- Sustainability
- Authentication
---
