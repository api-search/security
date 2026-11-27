---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: tripsy.app
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: tripsy.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tripsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripsy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tripsy
provider_slug: tripsy-app
slug: tripsy-app-domain-security
source_filename: tripsy-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripsy.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tripsy.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tripsy-app/security/tripsy-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel Planner
- Expense Tracking
- Calendar Sync
---
