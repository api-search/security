---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: colormind.io
  spf: true
hosts:
- cert_expires: Aug 16 16:54:20 2026 GMT
  host: colormind.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colormind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colormind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Colormind
provider_slug: colormind
slug: colormind-domain-security
source_filename: colormind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: colormind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:54:20 2026 GMT\n  hsts: false\ndomains:\n- domain: colormind.io\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colormind/refs/heads/main/security/colormind-domain-security.yml
summary_line: TLSv1.3
tags:
- Art And Design
- Public APIs
---
