---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: romaeris.com
  spf: true
hosts:
- cert_expires: Dec 17 04:20:30 2026 GMT
  host: romaeris.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Romaeris Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Romaeris Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Romaeris Corporation
provider_slug: romaeris-corporation
slug: romaeris-corporation-domain-security
source_filename: romaeris-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: romaeris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 04:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: romaeris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/romaeris-corporation/security/romaeris-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
