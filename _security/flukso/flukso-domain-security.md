---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flukso.net
  spf: false
hosts:
- cert_expires: Nov 29 10:16:07 2026 GMT
  host: flukso.net
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flukso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flukso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Flukso
provider_slug: flukso
slug: flukso-domain-security
source_filename: flukso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flukso.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 10:16:07 2026 GMT\n  hsts: false\ndomains:\n- domain: flukso.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flukso/security/flukso-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Monitoring
- IoT
- Utilities
---
