---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oltreilsolco.it
  spf: false
hosts:
- cert_expires: Feb  1 04:45:03 2027 GMT
  host: oltreilsolco.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oltre il Solco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oltre il Solco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Oltre il Solco
provider_slug: oltreilsolco-it
slug: oltreilsolco-it-domain-security
source_filename: oltreilsolco-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oltreilsolco.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 04:45:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oltreilsolco.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oltreilsolco-it/security/oltreilsolco-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Agriculture
- Water
- Italy
- Open Data
- Company
---
