---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 1acre.in
  spf: true
hosts:
- cert_expires: Dec 22 00:56:01 2026 GMT
  host: 1acre.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1Acre In Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1acre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 1acre
provider_slug: 1acre-in
slug: 1acre-in-domain-security
source_filename: 1acre-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1acre.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 00:56:01 2026 GMT\n  hsts: false\ndomains:\n- domain: 1acre.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/1acre-in/security/1acre-in-domain-security.yml
summary_line: TLSv1.3
tags:
- Real Estate
- LandMarketplace
- DataLayers
- India
- Developer Tools
---
