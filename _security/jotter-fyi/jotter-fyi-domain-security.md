---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jotter.fyi
  spf: false
hosts:
- cert_expires: Dec 16 03:27:10 2026 GMT
  host: jotter.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jotter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jotter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jotter
provider_slug: jotter-fyi
slug: jotter-fyi-domain-security
source_filename: jotter-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jotter.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 03:27:10 2026 GMT\n  hsts: false\ndomains:\n- domain: jotter.fyi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jotter-fyi/security/jotter-fyi-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- ChatGPT
- Claude
- Plugins
- Productivity
---
