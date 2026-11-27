---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cruisify.co.uk
  spf: false
hosts:
- cert_expires: Jan  6 11:08:28 2027 GMT
  host: cruisify.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cruisify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cruisify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Cruisify
provider_slug: cruisify-co-uk
slug: cruisify-co-uk-domain-security
source_filename: cruisify-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cruisify.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 11:08:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cruisify.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cruisify-co-uk/security/cruisify-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Cruise
- Comparison
- United Kingdom
- Platform
---
