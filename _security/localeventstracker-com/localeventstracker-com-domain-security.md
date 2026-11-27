---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: localeventstracker.com
  spf: false
hosts:
- cert_expires: Jan  6 17:59:11 2027 GMT
  host: localeventstracker.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: localeventstracker-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for localeventstracker-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: localeventstracker-com
provider_slug: localeventstracker-com
slug: localeventstracker-com-domain-security
source_filename: localeventstracker-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localeventstracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 17:59:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: localeventstracker.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/localeventstracker-com/security/localeventstracker-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Event
- Alerts
- AI Assistant
---
