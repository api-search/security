---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: certman.app
  spf: true
hosts:
- cert_expires: Dec 21 11:56:51 2026 GMT
  host: certman.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certman App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Certman
provider_slug: certman-app
slug: certman-app-domain-security
source_filename: certman-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certman.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 11:56:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: certman.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/certman-app/security/certman-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Certificate Authority
- PKI
- TLS
- Automation
---
