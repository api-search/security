---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: ohauth.ai
  spf: false
hosts:
- cert_expires: Dec 27 22:11:13 2026 GMT
  host: ohauth.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ohauth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oh Auth., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Oh Auth.
provider_slug: ohauth
slug: ohauth-domain-security
source_filename: ohauth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohauth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:11:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ohauth.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ohauth/security/ohauth-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
