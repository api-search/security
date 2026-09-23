---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aizenglobal.com
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: aizenglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aizenglobal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aizenglobal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aizenglobal
provider_slug: aizenglobal
slug: aizenglobal-domain-security
source_filename: aizenglobal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aizenglobal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aizenglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aizenglobal/refs/heads/main/security/aizenglobal-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Fintech
- AI
- DigitalBanking
- ESG
---
