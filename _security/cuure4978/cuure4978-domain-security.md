---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cuure.com
  spf: true
hosts:
- cert_expires: Dec  3 23:10:22 2026 GMT
  host: cuure.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuure4978 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuure4978, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cuure4978
provider_slug: cuure4978
slug: cuure4978-domain-security
source_filename: cuure4978-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cuure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:10:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cuure.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuure4978/refs/heads/main/security/cuure4978-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Supplements
- Personalised Health
- Biological Tests
- Tracking Technologies
- Science‑Backed
- French Lab
---
