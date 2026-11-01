---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: octotrip.app
  spf: false
hosts:
- cert_expires: Dec  8 15:31:11 2026 GMT
  host: octotrip.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octotrip App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for octotrip-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: octotrip-app
provider_slug: octotrip-app
slug: octotrip-app-domain-security
source_filename: octotrip-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octotrip.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 15:31:11 2026 GMT\n  hsts: false\ndomains:\n- domain: octotrip.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/octotrip-app/security/octotrip-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Travel
- MCP
- Flights
- RentalCars
---
