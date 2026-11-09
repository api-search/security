---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: constat-auto.com
  spf: false
hosts:
- cert_expires: Dec 27 09:41:41 2026 GMT
  host: constat-auto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constat Auto Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constat Auto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Constat Auto
provider_slug: constat-auto-com
slug: constat-auto-com-domain-security
source_filename: constat-auto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constat-auto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 09:41:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: constat-auto.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/constat-auto-com/security/constat-auto-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Vehicles
- Accident
- Reporting
- PDF
- French
---
