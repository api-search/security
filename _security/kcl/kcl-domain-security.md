---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kcl-lang.io
  spf: false
hosts:
- cert_expires: Sep 14 07:43:49 2026 GMT
  host: kcl-lang.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kcl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KCL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KCL
provider_slug: kcl
slug: kcl-domain-security
source_filename: kcl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kcl-lang.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kcl-lang.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kcl/refs/heads/main/security/kcl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Configuration Language
- Infrastructure as Code
- Policy as Code
---
