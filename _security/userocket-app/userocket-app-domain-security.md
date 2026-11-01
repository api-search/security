---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: userocket.app
  spf: false
hosts:
- cert_expires: Jan  4 17:17:45 2027 GMT
  host: userocket.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Userocket App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Rocket
provider_slug: userocket-app
slug: userocket-app-domain-security
source_filename: userocket-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userocket.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 17:17:45 2027 GMT\n  hsts: null\ndomains:\n- domain: userocket.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/userocket-app/security/userocket-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobile
- Web
- API
- Developer
---
