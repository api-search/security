---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orionhealth.io
  spf: false
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: developer.orionhealth.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orion Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orion Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orion Health
provider_slug: orion-health
slug: orion-health-domain-security
source_filename: orion-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.orionhealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: orionhealth.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion-health/refs/heads/main/security/orion-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Health
- Public APIs
---
