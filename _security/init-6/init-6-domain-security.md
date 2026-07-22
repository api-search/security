---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: init-6.fund
  spf: true
hosts:
- cert_expires: Oct  6 19:25:57 2026 GMT
  host: init-6.fund
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Init 6 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Init 6, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Init 6
provider_slug: init-6
slug: init-6-domain-security
source_filename: init-6-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: init-6.fund\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:25:57 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: init-6.fund\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/init-6/refs/heads/main/security/init-6-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
