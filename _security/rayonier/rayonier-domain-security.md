---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rayonier.com
  spf: true
hosts:
- cert_expires: Jan 28 23:27:10 2027 GMT
  host: www.rayonier.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: developer.rayonier.com
  https: false
- host: api.rayonier.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rayonier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rayonier, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rayonier
provider_slug: rayonier
slug: rayonier-domain-security
source_filename: rayonier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rayonier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:27:10 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.rayonier.com\n  https: false\n- host: api.rayonier.com\n  https: false\ndomains:\n- domain: rayonier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rayonier/refs/heads/main/security/rayonier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Timber
- Real Estate
- Forest Products
---
