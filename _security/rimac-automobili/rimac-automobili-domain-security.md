---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rimac-automobili.com
  spf: true
hosts:
- cert_expires: Mar  1 11:58:35 2027 GMT
  host: www.rimac-automobili.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rimac Automobili Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rimac Automobili, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rimac Automobili
provider_slug: rimac-automobili
slug: rimac-automobili-domain-security
source_filename: rimac-automobili-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rimac-automobili.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 11:58:35 2027 GMT\n  hsts: false\ndomains:\n- domain: rimac-automobili.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rimac-automobili/refs/heads/main/security/rimac-automobili-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Automotive
- Electric Vehicles
- Manufacturing
- Automotive Technology
- Hypercars
- Connected Vehicles
- Telematics
- Croatia
- Mobility
---
