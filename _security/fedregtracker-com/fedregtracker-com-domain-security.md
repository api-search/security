---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: fedregtracker.com
  spf: false
hosts:
- cert_expires: Jan  6 17:58:58 2027 GMT
  host: fedregtracker.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FedReg Tracker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FedReg Tracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FedReg Tracker
provider_slug: fedregtracker-com
slug: fedregtracker-com-domain-security
source_filename: fedregtracker-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fedregtracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 17:58:58 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fedregtracker.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fedregtracker-com/security/fedregtracker-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Federal
- Regulations
- Alerts
- Monitoring
---
