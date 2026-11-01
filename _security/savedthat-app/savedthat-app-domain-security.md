---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savedthat.app
  spf: true
hosts:
- cert_expires: Jan  6 05:30:41 2027 GMT
  host: savedthat.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Savedthat App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for savedthat-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: savedthat-app
provider_slug: savedthat-app
slug: savedthat-app-domain-security
source_filename: savedthat-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: savedthat.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 05:30:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: savedthat.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/savedthat-app/security/savedthat-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- AI
- Search
- Transcription
- Productivity
---
