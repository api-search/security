---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: flywhereto.com
  spf: false
hosts:
- cert_expires: Jan 23 16:02:42 2027 GMT
  host: flywhereto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flywhereto Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intuitive Bricks AB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Intuitive Bricks AB
provider_slug: flywhereto-com
slug: flywhereto-com-domain-security
source_filename: flywhereto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flywhereto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 16:02:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flywhereto.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flywhereto-com/security/flywhereto-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Travel
- Aviation
- Mapping
- DataVisualization
- OpenSource
---
