---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: octopad.app
  spf: false
hosts:
- cert_expires: Feb  5 16:12:01 2027 GMT
  host: octopad.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octopad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octopad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Octopad
provider_slug: octopad-app
slug: octopad-app-domain-security
source_filename: octopad-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octopad.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 16:12:01 2027 GMT\n  hsts: false\ndomains:\n- domain: octopad.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/octopad-app/security/octopad-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
