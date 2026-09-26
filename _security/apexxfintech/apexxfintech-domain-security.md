---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: equityzen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apexx.global
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: equityzen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 07:33:57 2026 GMT
  host: apexx.global
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Apexxfintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apexxfintech, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apexxfintech
provider_slug: apexxfintech
slug: apexxfintech-domain-security
source_filename: apexxfintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equityzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\n- host: apexx.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: equityzen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apexx.global\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/security/apexxfintech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- API
- Orchestration
- Global
---
