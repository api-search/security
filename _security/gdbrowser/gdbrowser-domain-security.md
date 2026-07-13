---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gdbrowser.com
  spf: false
hosts:
- cert_expires: Oct  3 03:29:37 2026 GMT
  host: gdbrowser.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gdbrowser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GDBrowser, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GDBrowser
provider_slug: gdbrowser
slug: gdbrowser-domain-security
source_filename: gdbrowser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gdbrowser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:29:37 2026 GMT\n  hsts: false\ndomains:\n- domain: gdbrowser.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gdbrowser/refs/heads/main/security/gdbrowser-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
