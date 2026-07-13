---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: github.blog
  spf: false
hosts:
- cert_expires: Sep 24 21:41:23 2026 GMT
  host: github.blog
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Git Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Git.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Git.io
provider_slug: git-io
slug: git-io-domain-security
source_filename: git-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: github.blog\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:41:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: github.blog\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/git-io/refs/heads/main/security/git-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- URL Shorteners
- Public APIs
---
