---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: file.io
  spf: true
hosts:
- cert_expires: Sep 23 07:35:19 2026 GMT
  host: www.file.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: File Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for File.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: File.io
provider_slug: file-io
slug: file-io-domain-security
source_filename: file-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.file.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:35:19 2026 GMT\n  hsts: false\ndomains:\n- domain: file.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/file-io/refs/heads/main/security/file-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud Storage And File Sharing
- Public APIs
---
