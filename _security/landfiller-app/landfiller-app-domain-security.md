---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: landfiller.app
  spf: false
hosts:
- cert_expires: Jan 25 11:56:28 2027 GMT
  host: landfiller.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: landfiller-app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for landfiller-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: landfiller-app
provider_slug: landfiller-app
slug: landfiller-app-domain-security
source_filename: landfiller-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landfiller.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 11:56:28 2027 GMT\n  hsts: false\ndomains:\n- domain: landfiller.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/landfiller-app/security/landfiller-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Mana calculator
- Card search
- Commander
- Land base builder
- Guides
---
