---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sunyur.com
  spf: true
hosts:
- cert_expires: Jan  7 08:12:38 2027 GMT
  host: www.sunyur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  7 08:12:38 2027 GMT
  host: open.sunyur.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sunyur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunyur, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sunyur
provider_slug: sunyur
slug: sunyur-domain-security
source_filename: sunyur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sunyur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 08:12:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.sunyur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 08:12:38 2027 GMT\n  hsts: false\ndomains:\n- domain: sunyur.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunyur/refs/heads/main/security/sunyur-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Procurement
- SRM
- E-Procurement
- Supplier Management
- Digital Procurement
- Enterprise Software
- SaaS
- B2B
- China
- AI
---
