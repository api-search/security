---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: motionmenu.ca
  spf: false
hosts:
- cert_expires: Jan 22 20:44:39 2027 GMT
  host: motionmenu.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Motion Menu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motion Menu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Motion Menu
provider_slug: motionmenu-ca
slug: motionmenu-ca-domain-security
source_filename: motionmenu-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motionmenu.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 20:44:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: motionmenu.ca\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/motionmenu-ca/security/motionmenu-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Motion
- UI
- Design
- Web
- Open Source
---
