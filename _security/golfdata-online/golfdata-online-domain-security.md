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
  domain: golfdata.online
  spf: true
hosts:
- cert_expires: Jan 17 01:25:41 2027 GMT
  host: golfdata.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GolfData Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GolfData Online, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GolfData Online
provider_slug: golfdata-online
slug: golfdata-online-domain-security
source_filename: golfdata-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golfdata.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 01:25:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: golfdata.online\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/golfdata-online/security/golfdata-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Golf
- Artificial Intelligence
- Sports
- Data
- Analytics
---
