---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: garagedoorman.ca
  spf: true
hosts:
- cert_expires: Dec 17 08:44:32 2026 GMT
  host: garagedoorman.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: garagedoorman-ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for garagedoorman-ca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: garagedoorman-ca
provider_slug: garagedoorman-ca
slug: garagedoorman-ca-domain-security
source_filename: garagedoorman-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: garagedoorman.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 08:44:32 2026 GMT\n  hsts: false\ndomains:\n- domain: garagedoorman.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/garagedoorman-ca/security/garagedoorman-ca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Garage Door Repair
- Garage Door Installation
- Opener Repair
- Annual Maintenance
- Residential Services
- Ontario
---
