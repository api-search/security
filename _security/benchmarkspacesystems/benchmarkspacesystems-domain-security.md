---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: benchmarkspacesystems.com
  spf: false
hosts:
- cert_expires: Nov 26 22:57:16 2026 GMT
  host: www.benchmarkspacesystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benchmarkspacesystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benchmarkspacesystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Benchmarkspacesystems
provider_slug: benchmarkspacesystems
slug: benchmarkspacesystems-domain-security
source_filename: benchmarkspacesystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchmarkspacesystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:57:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: benchmarkspacesystems.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchmarkspacesystems/refs/heads/main/security/benchmarkspacesystems-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Aerospace
- Propulsion
- Space
- Engineering
---
