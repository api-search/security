---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: changedetection.io
  spf: true
hosts:
- cert_expires: Dec 17 17:23:24 2026 GMT
  host: changedetection.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Changedetection Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for changedetection.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: changedetection.io
provider_slug: changedetection-io
slug: changedetection-io-domain-security
source_filename: changedetection-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: changedetection.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 17:23:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: changedetection.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/changedetection-io/security/changedetection-io-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Monitoring
- Webhooks
- Alerts
- OpenSource
---
