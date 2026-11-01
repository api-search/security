---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crossfireintegration.com
  spf: false
hosts:
- cert_expires: Dec  7 06:38:35 2026 GMT
  host: crossfireintegration.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crossfireintegration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sandfield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sandfield
provider_slug: crossfireintegration
slug: crossfireintegration-domain-security
source_filename: crossfireintegration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crossfireintegration.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 06:38:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crossfireintegration.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/crossfireintegration/security/crossfireintegration-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Integration
- EDI
- API
- Supply Chain
---
