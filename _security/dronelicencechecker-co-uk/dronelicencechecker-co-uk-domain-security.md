---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dronelicencechecker.co.uk
  spf: true
hosts:
- cert_expires: Jan  9 23:14:30 2027 GMT
  host: dronelicencechecker.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dronelicencechecker Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drone Licence Checker UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Drone Licence Checker UK
provider_slug: dronelicencechecker-co-uk
slug: dronelicencechecker-co-uk-domain-security
source_filename: dronelicencechecker-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dronelicencechecker.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:14:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dronelicencechecker.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dronelicencechecker-co-uk/security/dronelicencechecker-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Drone
- United Kingdom
- Aviation
- Regulations
---
