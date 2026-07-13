---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: navattic.com
  spf: true
hosts:
- cert_expires: Sep 20 04:35:49 2026 GMT
  host: www.navattic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 04:35:49 2026 GMT
  host: docs.navattic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 04:35:49 2026 GMT
  host: api.navattic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navattic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navattic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Navattic
provider_slug: navattic
slug: navattic-domain-security
source_filename: navattic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.navattic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:35:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.navattic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:35:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.navattic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:35:49 2026 GMT\n  hsts: null\ndomains:\n- domain: navattic.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/security/navattic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Interactive Demos
- Product Demo
- Sales Enablement
- Marketing
- No-Code
- Webhooks
- CRM Integration
- Sales Automation
---
