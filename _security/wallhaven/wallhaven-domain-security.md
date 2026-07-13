---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wallhaven.cc
  spf: true
hosts:
- cert_expires: Sep 12 08:29:03 2026 GMT
  host: wallhaven.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wallhaven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wallhaven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wallhaven
provider_slug: wallhaven
slug: wallhaven-domain-security
source_filename: wallhaven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wallhaven.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:29:03 2026 GMT\n  hsts: false\ndomains:\n- domain: wallhaven.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallhaven/refs/heads/main/security/wallhaven-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Photography
- Public APIs
---
