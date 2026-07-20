---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kodexglobal.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: kodexapi.com
  spf: false
hosts:
- cert_expires: Oct 14 06:32:04 2026 GMT
  host: www.kodexglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 01:36:33 2026 GMT
  host: docs.kodexapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: app.kodexglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kodex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kodex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kodex
provider_slug: kodex
slug: kodex-domain-security
source_filename: kodex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kodexglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:32:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kodexapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:36:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.kodexglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kodexglobal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kodexapi.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodex/refs/heads/main/security/kodex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Law Enforcement
- Compliance
- Legal
- Identity Verification
- Government
- Security
- Threat Intelligence
- Data Requests
- Trust and Safety
---
