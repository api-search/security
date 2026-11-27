---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: taprun.dev
  spf: true
hosts:
- cert_expires: Feb 19 09:32:02 2027 GMT
  host: taprun.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taprun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taprun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Taprun
provider_slug: taprun-dev
slug: taprun-dev-domain-security
source_filename: taprun-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taprun.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 09:32:02 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: taprun.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taprun-dev/security/taprun-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Browser Automation
- Local-first
- CLI
- Chrome Extension
---
