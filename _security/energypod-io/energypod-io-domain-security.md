---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: energypod.io
  spf: true
hosts:
- cert_expires: Jan 23 05:30:04 2027 GMT
  host: energypod.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EnergyPod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnergyPod, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EnergyPod
provider_slug: energypod-io
slug: energypod-io-domain-security
source_filename: energypod-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: energypod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 05:30:04 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: energypod.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/energypod-io/security/energypod-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Energy
- Podcasts
- Artificial Intelligence
- Weekly
- Media
---
