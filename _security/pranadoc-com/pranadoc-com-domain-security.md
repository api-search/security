---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: pranadoc.com
  spf: true
hosts:
- cert_expires: Dec 16 22:36:25 2026 GMT
  host: pranadoc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pranadoc Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prana Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Prana Health
provider_slug: pranadoc-com
slug: pranadoc-com-domain-security
source_filename: pranadoc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pranadoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 22:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pranadoc.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pranadoc-com/security/pranadoc-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
