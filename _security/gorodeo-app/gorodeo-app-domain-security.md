---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gorodeo.app
  spf: true
hosts:
- cert_expires: Apr 21 23:59:59 2027 GMT
  host: gorodeo.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gorodeo App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rodeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rodeo
provider_slug: gorodeo-app
slug: gorodeo-app-domain-security
source_filename: gorodeo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gorodeo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gorodeo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gorodeo-app/security/gorodeo-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Career
- JobSearch
- Startup
- Closed
---
