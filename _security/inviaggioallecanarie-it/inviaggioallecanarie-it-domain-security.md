---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inviaggioallecanarie.it
  spf: true
hosts:
- cert_expires: Feb  1 22:23:54 2027 GMT
  host: inviaggioallecanarie.it
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: In Viaggio alle Canarie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for In Viaggio alle Canarie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: In Viaggio alle Canarie
provider_slug: inviaggioallecanarie-it
slug: inviaggioallecanarie-it-domain-security
source_filename: inviaggioallecanarie-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inviaggioallecanarie.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 22:23:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inviaggioallecanarie.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inviaggioallecanarie-it/security/inviaggioallecanarie-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Vacation
- Canary Islands
- Artificial Intelligence
- Flights
---
