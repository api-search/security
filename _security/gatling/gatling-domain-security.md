---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gatling.io
  spf: true
hosts:
- cert_expires: Sep 29 08:44:46 2026 GMT
  host: gatling.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gatling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gatling
provider_slug: gatling
slug: gatling-domain-security
source_filename: gatling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatling.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gatling.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatling/refs/heads/main/security/gatling-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Load Testing
- Performance Testing
- Testing
---
