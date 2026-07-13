---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rossum.ai
  spf: true
hosts:
- cert_expires: Aug 21 04:57:15 2026 GMT
  host: rossum.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:17:28 2026 GMT
  host: elis.rossum.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:20:18 2026 GMT
  host: api.elis.rossum.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rossum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rossum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rossum
provider_slug: rossum
slug: rossum-domain-security
source_filename: rossum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rossum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 04:57:15 2026 GMT\n  hsts: false\n- host: elis.rossum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:17:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.elis.rossum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:20:18 2026 GMT\n  hsts: null\ndomains:\n- domain: rossum.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/security/rossum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document AI
- IDP
- Invoices
- OCR
- Workflow
- AP Automation
---
