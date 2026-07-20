---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lendo.sa
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: lendo.sa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 02:23:30 2026 GMT
  host: www.lendo.sa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.lendo.sa
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lendo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lendo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lendo
provider_slug: lendo
slug: lendo-domain-security
source_filename: lendo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lendo.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lendo.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 02:23:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lendo.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lendo.sa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendo/refs/heads/main/security/lendo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Crowdfunding
- Invoice Financing
- SME Finance
- Islamic Finance
- Saudi Arabia
- Middle East
---
