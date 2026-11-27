---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asipipes.com
  spf: false
hosts:
- cert_expires: Jan 15 17:15:09 2027 GMT
  host: asipipes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asipipes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asipipes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Asipipes
provider_slug: asipipes-com
slug: asipipes-com-domain-security
source_filename: asipipes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asipipes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 17:15:09 2027 GMT\n  hsts: null\ndomains:\n- domain: asipipes.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/asipipes-com/security/asipipes-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Pipelines
---
