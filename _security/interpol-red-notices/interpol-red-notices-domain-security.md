---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bund.dev
  spf: false
hosts:
- cert_expires: Sep 22 05:48:20 2026 GMT
  host: interpol.api.bund.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interpol Red Notices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interpol Red Notices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Interpol Red Notices
provider_slug: interpol-red-notices
slug: interpol-red-notices-domain-security
source_filename: interpol-red-notices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: interpol.api.bund.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:48:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bund.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interpol-red-notices/refs/heads/main/security/interpol-red-notices-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Government
- Public APIs
---
