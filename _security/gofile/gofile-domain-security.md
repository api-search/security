---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gofile.io
  spf: true
hosts:
- cert_expires: Sep 13 15:05:52 2026 GMT
  host: gofile.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gofile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoFile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GoFile
provider_slug: gofile
slug: gofile-domain-security
source_filename: gofile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gofile.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:05:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gofile.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gofile/refs/heads/main/security/gofile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Storage And File Sharing
- Public APIs
---
