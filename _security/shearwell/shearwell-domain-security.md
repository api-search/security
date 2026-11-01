---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shearwell.co.uk
  spf: true
hosts:
- cert_expires: Jan 26 10:30:40 2027 GMT
  host: shearwell.co.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shearwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shearwell Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shearwell Data
provider_slug: shearwell
slug: shearwell-domain-security
source_filename: shearwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shearwell.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 10:30:40 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: shearwell.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/shearwell/security/shearwell-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Livestock
- Animal Identification
- RFID
- Farm Management
- UK
---
