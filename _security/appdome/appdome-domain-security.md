---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appdome.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: appdome.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:48:59 2026 GMT
  host: apis.appdome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: fusion.appdome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appdome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appdome, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appdome
provider_slug: appdome
slug: appdome-domain-security
source_filename: appdome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appdome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: apis.appdome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fusion.appdome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appdome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdome/refs/heads/main/security/appdome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile App Security
- Mobile App Defense
- DevSecOps
- Application Security
- Mobile
- CI/CD
- App Signing
- Anti-Fraud
- Code Signing
---
