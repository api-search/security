---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dreamfare.app
  spf: true
hosts:
- cert_expires: Jan 30 21:50:15 2027 GMT
  host: dreamfare.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dreamfare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dreamfare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dreamfare
provider_slug: dreamfare-app
slug: dreamfare-app-domain-security
source_filename: dreamfare-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dreamfare.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 21:50:15 2027 GMT\n  hsts: false\ndomains:\n- domain: dreamfare.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dreamfare-app/security/dreamfare-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
