---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datausa.io
  spf: false
hosts:
- cert_expires: Aug 16 09:07:02 2026 GMT
  host: datausa.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data USA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Data USA
provider_slug: data-usa
slug: data-usa-domain-security
source_filename: data-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datausa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:07:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: datausa.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-usa/refs/heads/main/security/data-usa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Public APIs
---
