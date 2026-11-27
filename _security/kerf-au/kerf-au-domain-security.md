---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kerf.au
  spf: true
hosts:
- cert_expires: Jan 25 11:36:54 2027 GMT
  host: kerf.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kerf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kerf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kerf
provider_slug: kerf-au
slug: kerf-au-domain-security
source_filename: kerf-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kerf.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 11:36:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kerf.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kerf-au/security/kerf-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Waterjet
- Manufacturing
- Australia
- On-Demand
- Cutting
---
