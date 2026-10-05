---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apica.io
  spf: true
hosts:
- cert_expires: Nov 23 13:43:19 2026 GMT
  host: www.apica.io
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apica Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apica
provider_slug: apica-io
slug: apica-io-domain-security
source_filename: apica-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apica.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 13:43:19 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: apica.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apica-io/refs/heads/main/security/apica-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Observability
- Telemetry
- Artificial Intelligence
- Cloud
---
