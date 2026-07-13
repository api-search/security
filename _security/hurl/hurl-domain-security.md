---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: hurl.dev
  spf: true
hosts:
- cert_expires: Aug 25 21:02:56 2026 GMT
  host: hurl.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hurl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hurl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hurl
provider_slug: hurl
slug: hurl-domain-security
source_filename: hurl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hurl.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 21:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hurl.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hurl/refs/heads/main/security/hurl-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Command Line Interface
- HTTP Client
---
