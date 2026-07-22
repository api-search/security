---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lafraise.pro
  spf: true
hosts:
- cert_expires: Sep 29 18:19:01 2026 GMT
  host: lafraise.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Fraise Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Fraise Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: La Fraise Pro
provider_slug: la-fraise-pro
slug: la-fraise-pro-domain-security
source_filename: la-fraise-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lafraise.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lafraise.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-fraise-pro/refs/heads/main/security/la-fraise-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Dental
- Healthcare
- Health Tech
- Electronic Signature
- Patient Engagement
- SaaS
- France
- Practice Management
- Document Signing
---
