---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: globestudio.app
  spf: false
hosts:
- cert_expires: Dec 22 16:25:00 2026 GMT
  host: globestudio.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Globestudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globestudio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Globestudio
provider_slug: globestudio-app
slug: globestudio-app-domain-security
source_filename: globestudio-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globestudio.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 16:25:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: globestudio.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/globestudio-app/security/globestudio-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Mapping
- Visualization
- Open Source
- Cartography
- 3D
---
