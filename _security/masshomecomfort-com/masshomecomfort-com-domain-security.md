---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: masshomecomfort.com
  spf: true
hosts:
- cert_expires: Dec 26 19:51:48 2026 GMT
  host: masshomecomfort.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mass Home Comfort Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mass Home Comfort, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mass Home Comfort
provider_slug: masshomecomfort-com
slug: masshomecomfort-com-domain-security
source_filename: masshomecomfort-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: masshomecomfort.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:51:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: masshomecomfort.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/masshomecomfort-com/security/masshomecomfort-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Services
- Contractors
- Massachusetts
- Directory
- Free
---
